# Phan Thị Hồng Huế

### Date created: 
26/10/2025

### Project Title
Lab_Github

### Description
Thực hành các bài tập về **Git**

**1. Folk và Clone dự án**
- Folk dự án:
- Clone dự án:
```c
 git clone https://github.com/fhpthh/lab_github.git
```
**2. Thực hiện chỉnh sửa và quản lý phiên bản**
- Chỉnh sửa file README.md
- Thực hiện các lệnh 
```c
git add .
git commit -m"update"
git push -u origin main
```
**3. So sánh ***git merge*** và ***git rebase*****
**Git merge**
Tạo và di chuyển sang nhánh mới feature
```
git checkout -b feature
git add README.md
git commit -m "update branch feature"
```
- Quay trở lại nhánh main
```
git checkout main
git add README.md
git commit -m "update branch main"
```

- Dùng lệnh **git merge** để merge feature vào main
``` 
git merge feature -m "merge feature to main"
```

**Git rebase**
- Chuyển sang nhánh feature
- Cập nhật file README.md
- **git rebase main**

![Commit graph](images/gitrebase.png)

### So sánh giữa Merge và Rebase

| **Merge** | **Rebase** |
|------------|------------|
| `Git merge` là lệnh cho phép hợp nhất (merge) các nhánh trong Git. | `Git rebase` là lệnh cho phép tích hợp các thay đổi từ một nhánh này sang nhánh khác. |
| Trong **Git Merge**, nhật ký (log) sẽ hiển thị toàn bộ lịch sử của quá trình gộp commit. | Trong **Git Rebase**, nhật ký (log) là tuyến tính vì các commit được “phát lại” (rebase). |
| Tất cả các commit trên nhánh **feature** sẽ được kết hợp thành một commit duy nhất trên nhánh **master/main**. | Tất cả commit sẽ được **rebase** và giữ nguyên số lượng commit khi thêm vào nhánh **master/main**. |
| `Git merge` thường được dùng khi nhánh đích là **nhánh dùng chung (shared branch)**. | `Git rebase` thường được dùng khi nhánh đích là **nhánh cá nhân (private branch)**. |

**Commit graph**

![Commit graph](images/commitgraph.png)



### Files used
README.md

### Credits

