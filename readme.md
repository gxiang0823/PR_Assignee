### 1. 安装pandas和requests库
- 运行cmd，输入where python
- 在该路径下运行cmd，输入pip install pandas 和 pip install requests
- 等待安装完成，重启VScode
### 2. Run
- 现版本python脚本有四项输入：Release，PBU，Status和完整的cookie(不再是JSESSIONID=后面的部分)
- 依次输入脚本所需要的输入，等待十秒左右。
### 3. Result
- 脚本会生成一个名为Assignee_Info的.csv文件和一个result_release_status的版本txt文件
- .csv文件中存储的是当前版本PR的Dev的ID、Email和Leader_ID和Supervisor_ID信息。每次运行脚本并不会重新创建一个.csv文件，而是将新的Dev的信息更新到.csv文件中，重复的不会再更新进入.csv文件。
- result_release_status.txt文件存储的是当前版本PR的分配信息。
### 4. Other
- 代码在原始功能上新增了统计Assignee的信息的功能(包括姓名)，随着使用，数据积累会越来越完善。
- 新增了选择PBU的功能，不仅仅可以获取到CAM组的PR信息，别的group也可以使用。
- 在Fixed Plane Additive PRs for Sagar这一分组中有不正确情况，已修复。

