如何使用
```
sudo install -m 0755 -d /etc/apt/keyrings
curl -sSL https://xiaotong6666.github.io/zfs-deb-build/repo.asc | sudo gpg --dearmor -o /etc/apt/keyrings/zfs-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/zfs-archive-keyring.gpg] https://xiaotong6666.github.io/zfs-deb-build/ nightly main" | sudo tee /etc/apt/sources.list.d/zfs.list > /dev/null
```
单行复制
```
sudo install -m 0755 -d /etc/apt/keyrings
```
```
curl -sSL https://xiaotong6666.github.io/zfs-deb-build/repo.asc | sudo gpg --dearmor -o /etc/apt/keyrings/zfs-archive-keyring.gpg
```
```
echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/zfs-archive-keyring.gpg] https://xiaotong6666.github.io/zfs-deb-build/ nightly main" | sudo tee /etc/apt/sources.list.d/zfs.list > /dev/null
```
