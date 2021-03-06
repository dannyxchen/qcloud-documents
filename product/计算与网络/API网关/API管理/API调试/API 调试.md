通过 API 调试页面，您可以在配置完 API 后立即验证 API 的正确性，发起模拟 API 调用并查看具体调用日志和请求响应。如果 API 未按照您期望的方式工作，可以根据日志和响应，重新修改配置以符合您的设计期望。

1.在服务页面的 API 管理标签页中，选择需要调试的 API，单击右上角的【API调试】按钮，可以进入调试页面。
![调试](//mc.qcloudimg.com/static/img/d158bddcf804dd5ed670572d776d5ada/image.png)

2. 在调试页面，您可以看到需调试 API 的前端配置信息，包括路径、请求方法和请求参数。在请求参数位置，如果您配置了参数具有默认值，则默认值会默认填充到输入框中；如果您配置了参数必填，则在测试前会检查是否已填写必填参数；如果您的请求方法为 POST、PUT、DELETE，则会有 Body 参数需要您填写。
![调试](//mc.qcloudimg.com/static/img/9d95ca1579a8fefa2bb0f11be7b2355f/image.png)
>?如果非必填参数，用户不填写任何参数，则默认 API 网关会给后端传一个 null。

3. 单击【发送请求】后，您能看到两部分输出：
   1）请求日志：日志能详细输出您的请求记录，包括前端参数组装后的请求路径和方法，Headers 参数，后端实际调用的配置，向后端发起请求的过程和后端响应的响应码、数据内容。 
   2）响应：API 调用后实际返回给前端的响应码和数据内容。
![调试结果](//mc.qcloudimg.com/static/img/e84bc7854788295b9fe0b05e8791d019/image.png)
