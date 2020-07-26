# test

# Quy trình
- Clone repo về
- Tạo branch mới và checkout 
```bash
git checkout -b branch1
```
- Sau khi làm các thứ thì commit với thêm messages thôi
```bash
git add . 
git commit -m "messages..."
```
```bash
git commit -a -m "message..."
```
- Sau khi commit xong xuôi thì phải kiểm tra xem lại xem trong thời gian mình làm có gì mới ở nhánh master k
```bash
git checkout master
git fetch                 // Lấy thông tin về những cái mới
git diff ...origin        // Xem sự khác nhau giữa mới và cũ

git pull 
git checkout branch1
git merge master          //merge master về lại branch, sau đó commit lại, rồi đẩy lên remote ( origin)
git commit -a -m "message..."
git push origin branch1
```
- Sau khi push lên thì vào lại Github.com ấy rồi vào nhánh của mình chọn pull request rồi đợi cái PR đấy được verify rồi merged vào code chính. Sau khi merged thành công thì xóa branch cũ đi, tạo branch mới để làm
```bash 
git branch -d branch1
```
