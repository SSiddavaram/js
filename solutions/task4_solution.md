```
var randomItems = [];

randomItems.push({ one: 1, two: "two", three: function() { return 3; } });
randomItems.push("apple");
randomItems.push(void 0);
randomItems.push(null);
randomItems.push(100);
randomItems.push(function() {
  var foo = "bar";

  return foo;
});
```

Accessing random items:
```
for(x in randomItems)
  {
    console.log(randomItems[x])
  }
```

Results:
```
{
  "one": 1,
  three: function(),
  "two": "two"
}
apple
undefined
null
100
function () {
  var foo = "bar";

  return foo;
}
function (){
				return lower;
			}
function Array() { [native code] }
function (fn, bind){
		Array.forEach(this, fn, bind);
		return this;
	}
function (){
	var i = this.length, clone = new Array(i);
	while (i--) clone[i] = cloneOf(this[i]);
	return clone;
}
function (){
		return this.filter(function(item){
			return item != null;
		});
	}
function (methodName){
		var args = Array.slice(arguments, 1);
		return this.map(function(item){
			return item[methodName].apply(item, args);
		});
	}
function (keys){
		var obj = {}, length = Math.min(this.length, keys.length);
		for (var i = 0; i < length; i++) obj[keys[i]] = this[i];
		return obj;
	}
function (object){
		var result = {};
		for (var i = 0, l = this.length; i < l; i++){
			for (var key in object){
				if (object[key](this[i])){
					result[key] = this[i];
					delete object[key];
		…
function (item, from){
		return this.indexOf(item, from) != -1;
	}
function (array){
		this.push.apply(this, array);
		return this;
	}
function (){
		return (this.length) ? this[this.length - 1] : null;
	}
function (){
		return (this.length) ? this[Number.random(0, this.length - 1)] : null;
	}
function (item){
		if (!this.contains(item)) this.push(item);
		return this;
	}
function (array){
		for (var i = 0, l = array.length; i < l; i++) this.include(array[i]);
		return this;
	}
function (item){
		for (var i = this.length; i--;){
			if (this[i] === item) this.splice(i, 1);
		}
		return this;
	}
function (){
		this.length = 0;
		return this;
	}
function (){
		var array = [];
		for (var i = 0, l = this.length; i < l; i++){
			var type = typeOf(this[i]);
			if (type == 'null') continue;
			array = array.concat((type == 'array' || type == 'coll…
function (){
		for (var i = 0, l = this.length; i < l; i++){
			if (this[i] != null) return this[i];
		}
		return null;
	}
function (array){
		if (this.length != 3) return null;
		var rgb = this.map(function(value){
			if (value.length == 1) value += value;
			return value.toInt(16);
		});
		return (array) ? rgb : 'rgb(' …
function (array){
		if (this.length < 3) return null;
		if (this.length == 4 && this[3] == 0 && !array) return 'transparent';
		var hex = [];
		for (var i = 0; i < 3; i++){
			var bit = (this[i] - 0).…
function (array){
		this.push.apply(this, array);
		return this;
	}
function (){
		return Math.min.apply(null, this);
	}
function (){
		return Math.max.apply(null, this);
	}
function (){
		return this.length ? this.sum() / this.length : 0;
	}
function (){
		var result = 0, l = this.length;
		if (l){
			while (l--) result += this[l];
		}
		return result;
	}
function (){
		return [].combine(this);
	}
function (){
		for (var i = this.length; i && --i;){
			var temp = this[i], r = Math.floor(Math.random() * ( i + 1 ));
			this[i] = this[r];
			this[r] = temp;
		}
		return this;
	}
function (prop){
		return this.map(function(item){
			return item[prop];
		});
	}
function (){
		var red = this[0],
				green = this[1],
				blue = this[2],
				hue = 0;
		var max = Math.max(red, green, blue),
				min = Math.min(red, green, blue);
		var delta = max - min;
		var bri…
function (){
		var br = Math.round(this[2] / 100 * 255);
		if (this[1] == 0){
			return [br, br, br];
		} else {
			var hue = this[0] % 360;
			var f = hue % 60;
			var p = Math.round((this[2] * (100 …
undefined
```
