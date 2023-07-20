# ![image-20230716222650449](Ajax强化.assets/image-20230716222650449.png)1.Ajax强化

![image-20230716220801584](Ajax强化.assets/image-20230716220801584.png)

![image-20230716220830768](Ajax强化.assets/image-20230716220830768.png)

## 1. XMLHttpRequest的基本使用

### 1.1 什么是XMLHttpRequest

 ![image-20230716221203214](Ajax强化.assets/image-20230716221203214.png)

### 1.2 使用xhr发起GET请求

![image-20230716221338110](Ajax强化.assets/image-20230716221338110.png)

![image-20230716221411303](Ajax强化.assets/image-20230716221411303.png)

### 1.3 了解xhr对象的readyState属性

![image-20230716222212314](Ajax强化.assets/image-20230716222212314.png)

### 1.4 使用xhr发起带参数的GET请求

![image-20230716222318977](Ajax强化.assets/image-20230716222318977.png)

### 1.5 查询字符串



![image-20230716222540545](Ajax强化.assets/image-20230716222540545.png)

![image-20230716222916322](Ajax强化.assets/image-20230716222916322.png)

### 1.6 URL编码与解码

![image-20230716222930049](Ajax强化.assets/image-20230716222930049.png)

![image-20230717085149890](Ajax强化.assets/image-20230717085149890.png)

![image-20230717085240217](Ajax强化.assets/image-20230717085240217.png)

### 1.7 使用xhr发起POST请求

###  ![image-20230717090335087](Ajax强化.assets/image-20230717090335087.png)

![image-20230717090431691](Ajax强化.assets/image-20230717090431691.png)

## 2. 数据交换格式

### 2.1 什么是数据交换格式

 ![image-20230717094837388](Ajax强化.assets/image-20230717094837388.png)

### 2.2 XML

![image-20230717095048959](Ajax强化.assets/image-20230717095048959.png)

![image-20230717095026960](Ajax强化.assets/image-20230717095026960.png)

![image-20230717095131904](Ajax强化.assets/image-20230717095131904.png)

### 2.3 JSON

![image-20230717095915719](Ajax强化.assets/image-20230717095915719.png)

![image-20230717100322712](Ajax强化.assets/image-20230717100322712.png)

![image-20230717100356800](Ajax强化.assets/image-20230717100356800.png)

![image-20230717101152636](Ajax强化.assets/image-20230717101152636.png)![image-20230717101445258](Ajax强化.assets/image-20230717101445258.png)

![image-20230717101736683](Ajax强化.assets/image-20230717101736683.png)

![image-20230717101908140](Ajax强化.assets/image-20230717101908140.png)

## 3. 封装自己的Ajax函数

### 3.1 实现的效果

![image-20230717102046894](Ajax强化.assets/image-20230717102046894.png)

### 3.2 定义options参数选项

![image-20230717102158245](Ajax强化.assets/image-20230717102158245.png)

### 3.3 处理data参数

![image-20230717102314501](Ajax强化.assets/image-20230717102314501.png)

### 3.4 自定义函数

![image-20230717102502125](Ajax强化.assets/image-20230717102502125.png)

### 3.5  判断请求的类型

![image-20230717102602458](Ajax强化.assets/image-20230717102602458.png)



## 4. XMLHttpRequest Level2的新特性

### 4.1 XMLHttpRequest Level2

![image-20230717103012632](Ajax强化.assets/image-20230717103012632.png)

![image-20230717103050396](Ajax强化.assets/image-20230717103050396.png)

### 4.2 设置HTTP请求时限

![image-20230717103158011](Ajax强化.assets/image-20230717103158011.png)

### 4.3 FormData对象管理表单数据

![image-20230717104941749](Ajax强化.assets/image-20230717104941749.png)

![image-20230717105251905](Ajax强化.assets/image-20230717105251905.png)

### 4.4 上传文件

![image-20230717105447651](Ajax强化.assets/image-20230717105447651.png)

![image-20230717105522547](Ajax强化.assets/image-20230717105522547.png)

![image-20230717105640482](Ajax强化.assets/image-20230717105640482.png)

![image-20230717110028721](Ajax强化.assets/image-20230717110028721.png)

![image-20230717110210573](Ajax强化.assets/image-20230717110210573.png)

![image-20230717110255572](Ajax强化.assets/image-20230717110255572.png)

### 4.5 显示文件的上传进度

![image-20230717110956664](Ajax强化.assets/image-20230717110956664.png)

+ 拓展（选择上传的网速）
  + ![image-20230717111147992](Ajax强化.assets/image-20230717111147992.png)

+ 导入需要的库（bootstrap）

![image-20230717112315456](Ajax强化.assets/image-20230717112315456.png)

![image-20230717112745814](Ajax强化.assets/image-20230717112745814.png)

## 5. jQuery高级用法

### 5.1 jQuery实现文件上传

![image-20230717113014753](Ajax强化.assets/image-20230717113014753.png)

![image-20230717113102274](Ajax强化.assets/image-20230717113102274.png)

![image-20230717113250180](Ajax强化.assets/image-20230717113250180.png)

![image-20230717113414932](Ajax强化.assets/image-20230717113414932.png)

+++

>**要使用 jQuery 和 Bootstrap 实现文件上传以及结合进度条显示上传进度，可以按照以下步骤进行操作：**
>
>1. 引入 jQuery 和 Bootstrap 的库文件。在 HTML 文件的 `<head>` 部分添加如下代码：
>
>```html
><link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
><script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
>```
>
>2. 在 HTML 页面中添加一个文件选择输入框、上传按钮和进度条。例如：
>
>```html
><input type="file" id="fileInput">
><button id="uploadButton" class="btn btn-primary">上传文件</button>
><div class="progress mt-3" style="display: none;">
>  <div id="progressBar" class="progress-bar progress-bar-striped" role="progressbar" style="width: 0%" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100"></div>
></div>
>```
>
>3. 使用 jQuery 编写上传文件的 JavaScript 代码。在页面加载完成后，添加如下代码：
>
>```javascript
>$(document).ready(function() {
>  // 上传按钮点击事件
>  $('#uploadButton').click(function() {
>    var fileInput = $('#fileInput')[0];
>    var file = fileInput.files[0];
>    uploadFile(file);
>  });
>
>  // 上传文件函数
>  function uploadFile(file) {
>    var formData = new FormData();
>    formData.append('file', file);
>
>    $.ajax({
>      url: 'upload.php', // 后端处理上传的脚本地址
>      type: 'POST',
>      data: formData,
>      processData: false,
>      contentType: false,
>      xhr: function() {
>        var xhr = new window.XMLHttpRequest();
>        xhr.upload.addEventListener('progress', function(e) {
>          if (e.lengthComputable) {
>            var percent = Math.round((e.loaded / e.total) * 100);
>            $('#progressBar').width(percent + '%');
>            $('#progressBar').attr('aria-valuenow', percent);
>            $('#progressBar').text(percent + '%');
>          }
>        });
>        return xhr;
>      },
>      success: function(response) {
>        // 处理上传成功后的响应
>        console.log('上传成功');
>      },
>      error: function() {
>        // 处理上传失败后的响应
>        console.log('上传失败');
>      }
>    });
>  }
>});
>```
>
>4. 在后端编写处理上传文件的脚本。在示例中，我们将上传的文件通过 POST 请求发送到 `upload.php` 脚本进行处理。你需要根据实际情况编写后端脚本来保存上传的文件。
>
>请注意，示例中的代码仅展示了如何使用 jQuery 和 Bootstrap 实现文件上传和进度条显示上传进度的基本逻辑。在实际应用中，你可能需要进行更多的错误处理、安全性验证和其他功能的添加。
>
>上述代码中的 `upload.php` 文件是一个占位符，你需要根据自己的需求编写真实的后端处理逻辑来保存上传的文件。
>
>希望这个示例能帮助到你实现文件上传并结合进度条显示上传进度。如果有任何问题，请随时提问。

+++

### 5.2 jQuery实现loading效果

![image-20230717114049600](Ajax强化.assets/image-20230717114049600.png)

![image-20230717114203450](Ajax强化.assets/image-20230717114203450.png)

## 6. axios

### 6.1 什么是axios

![image-20230717114347722](Ajax强化.assets/image-20230717114347722.png)

###  6.2 axios发起GET请求

 ![image-20230717114502786](Ajax强化.assets/image-20230717114502786.png)

### 6.3 axios发起POST请求

![image-20230717114711776](Ajax强化.assets/image-20230717114711776.png)

### 6.4 直接使用axios发起请求

![image-20230717114927155](Ajax强化.assets/image-20230717114927155.png)

![image-20230717114904484](Ajax强化.assets/image-20230717114904484.png)