# crsync
a C library of Client-side rsync over HTTP via curl

## Guide
<<<<<<< HEAD
基于rsync算法的客户端二进制增量差异更新组件  
1. 纯C语言实现, 使用libcurl HTTP通讯，跨平台兼容性良好。  
2. 客户端使用rsync算法计算与服务器新版本的二进制差异，并增量下载更新数据。  
3. 服务器仅需支持HTTP File传输，普通CDN即可，无须搭建rsyncd。  
4. 目前已支持Android，Windows，理论上支持所有平台。  
5. 源码简单易懂，核心部分仅1000行，可随意扩展修改。  

## Workflow
+ 服务端生成新版本的摘要文件, 并部署到HTTP FileServer
+ 客户端使用libcurl下载资源，断点续传。
+ 客户端计算文件版本差异，增量下载差异内容并合并到本地。
+ 客户端附带一个轻量级版本控制策略组件。

## Android Build
+ Run `src/crsync-build.cmd`, output `src/libs/TARGET_ARCH_ABI/libcrsync.so`.

## Qt MinGW Build
+ build `src/crsync.pro`, output `src/m32/crsync.exe`
=======
鍩轰簬rsync绠楁硶鐨勫鎴风浜岃繘鍒跺閲忓樊寮傛洿鏂扮粍浠�  
1. 绾疌璇█瀹炵幇, 浣跨敤libcurl HTTP閫氳锛岃法骞冲彴鍏煎鎬ц壇濂姐��
2. 瀹㈡埛绔娇鐢╮sync绠楁硶璁＄畻涓庢湇鍔″櫒鏂扮増鏈殑浜岃繘鍒跺樊寮傦紝骞跺閲忎笅杞界儹鏇存柊銆�  
3. 鏈嶅姟鍣ㄤ粎闇�鏀寔HTTP File浼犺緭锛屾櫘閫欳DN鍗冲彲锛屾棤椤绘惌寤簉syncd銆�  
4. 鐩墠宸叉敮鎸丄ndroid锛學indows锛岀悊璁轰笂鏀寔鎵�鏈夊钩鍙般��  
5. 婧愮爜绠�鍗曟槗鎳傦紝鏍稿績閮ㄥ垎浠�1000琛岋紝鍙殢鎰忔墿灞曚慨鏀广��  

## Workflow
+ 瀹㈡埛绔娇鐢╨ibcurl涓嬭浇璧勬簮锛屾柇鐐圭画浼犮��
+ 瀹㈡埛绔绠楁枃浠剁増鏈樊寮傦紝澧為噺涓嬭浇宸紓鍐呭骞跺悎骞跺埌鏈湴銆�
+ 杞婚噺绾х増鏈帶鍒剁瓥鐣ョ粍浠躲��
>>>>>>> f862d07b7d68010f0f4dee18abfa180b3bbb69fb
