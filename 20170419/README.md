# 2장
기본적인 패턴 이해

## 객체
```bash
	var first_object = {
		name : "tae woong"
		, result : function() {
			console.log(this.name + " : " +this.calc(3));
		}
	}
	first_object.result();
```

## 프로토타입
```bash
	var example = function(){
		this.name = "tae woong";
		this.calc = function(param) {
			return param + 5;
		};
	}

	example.prototype.result = function() {
			console.log(this.name + " : " + this.calc(3));
		};
	var instance = new example();
	instance.result();
```

## 상속
상속이란 개념은 없고 프로토타입 결합 ! 
```bash
	function clone(source, destination) {
		for(var attr in source.prototype) {
			destination.prototype[attr] = source.prototype[attr];
		}
	}
```

## 모듈
```
	westeros.module = example;

	var module = new westeros.module();
	module.result();
```

## 모듈2
2장에서 가장 중요한 부분 구조적으로 생각이 많이 필요
```
	}) (westeros.structures || (westeros.structures = {}));
			return westeros.structures.module.result() + " " + westeros.structures.method.result();
		}) (westeros || (westeros = {}));
```