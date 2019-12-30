# 使用v2ray实现科学上网



这里我用的是vultr家的vps

[网址在这里](https://www.vultr.com/)

自行注册登录



1. 充钱

   点图中红色圈中内容

   ![](C:\Users\Shanya\Desktop\1.png)

2. 自行选择支付方式和金额（可用微信、支付宝）

   

   ![](C:\Users\Shanya\Desktop\2.png)

3. 充完后点击红圈中内容去选择服务器

   ![](C:\Users\Shanya\Desktop\3.png)

4. 点击加号添加服务器

   ![](C:\Users\Shanya\Desktop\4.png)

5. 依次选择 Cloud Compute

   ​				New York（NJ）

   ​				Ubuntu18.04 x64

   ​				$2.5/mo

   其他默认不管

6. 依次点击

   ![](C:\Users\Shanya\Desktop\3.png)

   ![](C:\Users\Shanya\Desktop\6.png)

   ![](C:\Users\Shanya\Desktop\7.png)

7. 会显示 出服务器的信息

   ![](C:\Users\Shanya\Desktop\8.png)

8. 百度搜索XShell并下载安装

   打开 Xshell

   ![1577705872214](C:\Users\Shanya\AppData\Roaming\Typora\typora-user-images\1577705872214.png)

9. 点击新建

   ![](C:\Users\Shanya\Desktop\9.png)

10. 在主机处输入你服务器的IP地址（第二张图片上的涂黑处）

    ![](C:\Users\Shanya\Desktop\10.png)

    ![](C:\Users\Shanya\Desktop\8.png)

11. 点击连接（之后敲回车等到出现下面这个对话框）

    ![1577706138979](C:\Users\Shanya\AppData\Roaming\Typora\typora-user-images\1577706138979.png)

12. 输入root

13. 密码 在图中的黑点处

    ![](C:\Users\Shanya\Desktop\8.png)

14. 出现此则 代表连接成功

    ![1577706267556](C:\Users\Shanya\AppData\Roaming\Typora\typora-user-images\1577706267556.png)

15. 输入

    ```
    wget https://install.direct/go.sh
    ```

    ```
    sudo bash go.sh
    ```

    ```
    sudo systemctl start v2ray
    ```

    

    








