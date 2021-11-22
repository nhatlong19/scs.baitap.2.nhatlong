# I - Setup

### 1. Clone repo
```
git clone git@github.com:noothaithinh/scs.baitap.2.git
cd scs.baitap.2.git
sh ./install.sh
```
### 2. Đổi URL
```
git remote set-url origin git@github.com:nhatlong19/scs.baitap.2.nhatlong.git
```

# II - Giai bai tap:

## 1. Thêm file .gitignore

Run command:
```
vim .gitignore
```
thêm các file .env và tmp


## 2. Tạo pull request

### Push code lên các nhánh
Run command:
```
git checkout develop
git add .
git commit -m "push code to master"
git push origin master

git checkout develop
git add .
git commit -m "push code to develop"
git push origin develop
```
### Copy branch **< release >** từ  **< master >**
Run command:
```
git checkout -b release master
```

### Tạo Pull Request để Merge branch **< develop >** vào **< release >** 

Sẽ sinh ra conflict ở bước này, ta cần Resolve

### Tạo Pull Request để Merge branch **< release >**  vào **< master >** 
