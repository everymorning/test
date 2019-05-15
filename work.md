## 数组和函数作业
### 第一题
        // 第一题:倒叙
        function num(){			//封装成函数
        var arr = [8, 99, 46, 72, 4];	//定义一个数组
        for (i = arr.length - 1; i >= 0; i--) {	//arr.length-1:角标0-4
            console.log(arr[i])
        }  
        }
        num()			//调用
### 第二题
        第二题
        function letter() {			//封装成函数
            var arr = ['a', 's', 'd', 'f'];
            var x = prompt("请输入一个字母")
            for (i = 0; i < arr.length; i++) {	//i < arr.length:比较最大值-1次
                if (x == arr[i]) {		//输入的数和数组其中一个相同
                    alert("有");
                    break;		//弹出有并且停止循环
                } else if (i == arr.length - 1) {	//循环一轮并且没有相同的
                    alert("无");
                }
            }
        }
        letter()
### 第三题
        第三题:素数
        function num(){
        var num = prompt("输入一个数");
        var a = 0;		//存储每个能整除的数
        for (i = 1; i <= num; i++) {
            if (num % i == 0) {		//输入的数和第1次循环取余,直到和自身相除
                a++
            }
        } if (a == 2) {		//除数个数只有两个
            alert("质数")
        } else {
            alert("不是")
        }  
        }
        num()
### 第四题
        // 第四题 排序
        function num(){
        var arr = [8, 99, 46, 72, 5];
        for (i = 0; i < arr.length - 1; i++) {	//控制对比轮数
            for (j = 0; j < arr.length - 1 - i; j++) {	//每轮对比次数(每对比一轮减去轮数)
                if (arr[j] < arr[j + 1]) {	//如果每次对比的数小于数组里的数
                    var temp = arr[j];		//那么把这个数先存到空数组里
                    arr[j] = arr[j + 1];	//把比它小的数放到它的位置
                    arr[j + 1] = temp;		//把空盒子里的较大的数放到后面
                }
            }
        } console.log(arr)    
        }
        num()
### 第五题
        // 第五题
        var temp = [];			//需要一个空数组,放挑出来的值
        var money = [1500, 1200, 2000, 2100, 1800];	
        for (i = 0; i < money.length; i++) {	                                                                                  
            if (money[i] <= 2000) {		//如果这个值小于2000
                temp.push(money[i])		//把这个数正序放到temp里
            }
        } alert(temp)
### 第六题
		// 第六题
        var sum1 = 1;			//第一个月,1对
        var sum2 = 1;			//第二个月,还是1对
        var sum3 = 0;			//第三个月,2对(三个月生一对)等于前两个月的和
        for (i = 3; i <= 22; i++) {		//从第三个月开始循环,到22个月结束
            sum3 = sum1 + sum2;		//第三个月等于前两个月的和
            sum1 = sum2;			//把第二个月的值作为下一次循环的第一个值
            sum2 = sum3;			//把第三个月的值作为下一次循环的第二个值
        } alert(sum3)
### douban.js作业
		先引入js文件 src="./douban.js"
            console.log(movies);
            var sub=movies.subjects;	//sub存储movies下的subjects
            console.log(sub);
            var str="";			//空字符串接收数据
            for(i=0;i<sub.length;i++){		//遍历
                str+=sub[i].title+" 导演:";		
                var dir=sub[i].directors
                for(var j=0;j<dir.length;j++){
                    str+=dir[j].name+" year:";
                    
                }
            var year=sub[i].year
                for(var y=0;y<year.length;y++){
                str+=year[y]+""
			}
            console.log(str)
            str=""
            }
### 创建对象
			// 创建对象的第一种方式 构造函数
			var obj = new Object();
			obj.name = "张三";
			obj.age = 20;
			obj.say = function (){
				alert(this.name);
			}
			console.log(obj);
			console.log(obj.name);
			obj.say();
			
			// 创建对象的第二种方式
			var obj = {};
			obj.name = "张三";
			obj.age = 20;
			obj.say = function (){
				alert(this.name + "的年龄为" + this.age);
			}
			obj.say();