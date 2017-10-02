
This is hw1 A) Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f (master) $ git branch test1

Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f (master) $ git branch test2 D) Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (test1) $ git add test.txt warning: LF will be replaced by CRLF in hw/test.txt. The file will have its original line endings in your working directory. $ git commit test.txt warning: LF will be replaced by CRLF in hw/test.txt. The file will have its original line endings in your working directory. [test1 addd2dc] all good 1 file changed, 1 insertion(+) create mode 100644 hw/test.txt E) The file isn't the test2 branch because the test.txt file was created in the test1 branch. G) $ git checkout test1 error: The following untracked working tree files would be overwritten by checkout: hw/test.txt Please move or remove them before you switch branches. Aborting Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (test2) $ rm test.txt

Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (test2) $ ls readme.md

Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (test2) $ git checkout test1 Switched to branch 'test1' A hw/.readme.md.swp

Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (test1) $ git merge master Already up-to-date. H) $ git merge test1 Updating a460f86..addd2dc Fast-forward hw/test.txt | 1 + 1 file changed, 1 insertion(+) create mode 100644 hw/test.txt I) Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (master) $ git checkout test1 Switched to branch 'test1' A hw/.readme.md.swp J)Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (master) $ git merge test2 Updating addd2dc..6955ba3 Fast-forward hw/test.txt | 2 +- 1 file changed, 1 insertion(+), 1 deletion(-) O) Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (test2) $ git branch -d test1 Deleted branch test1 (was addd2dc). P) Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (master) $ git branch -d test1 error: branch 'test1' not found.

Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (master) $ git branch

master test2 R) Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (test2) $ git branch -d test2 error: Cannot delete branch 'test2' checked out at 'C:/Users/Trevor/Git/ICP2017F' S)Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (master) $ git branch -d test2 Deleted branch test2 (was 6955ba3).
Trevor@DESKTOP-GMSO2QR MINGW64 ~/git/icp2017f/hw (master) $ git branch

maste\r
