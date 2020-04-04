##JavaScript Comment & Documentation Style Guide

Comment တခုကို code ရဲ့ရည်ရွယ်ချက်က ဘာလဲနဲ့ ဘာလို့ဒီလိုပုံစံ code ရေးထားရတာလဲဆိုတာရှင်းပြရင်အကောင်းဆုံးပါ။

ဒီနေရာမှာcode documentation လုပ်ဖို့သုံးတဲ့ jsdoc cli ကိုညွန်းပေးပါရစေ။ သူ့ထဲမှာပါတဲ့ annotations တွေကို code documentation လုပ်ဖို့အတွက် သုံးလို့ရပါတယ်။ ဒီနေရာမှာတော့ အဲ့ထဲက annotations အချို့ကိုပဲသုံးဖို့ညွန်းပရစေ။
- @constructor: ဒါကတော့ class သို့မဟုတ် new keyword ခေါ်လို့ရမယ့် function တခုရှေ့မှာသုံးပါတယ်။
- @description: ဒီfunctionက ဘာလဲဆိုတာ ဖေယ်ပြဖို့သုံးပါတယ်။ HTML tag တွေကိုသုံးချင်ရင်လည်း ရပါတယ်။
- @param: function တခုရဲ့ parameterရဲ့ နာမည်၊ type နဲ့ဘာလဲဆိုတာအကြမ်းဖော်ပြဖို့သုံးပါတယ်။
- @returns: return ပြန်မယ့် type နဲ့ description ရေးဖို့သုံးပါတယ်။

ပထမဥပမာ။ **class constructor**
```js
/** * @description Represents a book 
    * @constructor 
    * @param {string} title - The title of the book 
    * @param {string} author - The author of the book 
*/ 
function Book(title, author) { ... }
```
ဒုတိယဥပမာ။ **function**
```js
/** * @description Adds two numbers 
    * @param {number} a 
    * @param {number} b 
    * @returns {number} Sum of a and b 
*/ 
function sum(a, b) { return a + b; }
```