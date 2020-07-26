# matplotlib-selfstudy
## The original tutorial can be found [here](https://www.youtube.com/playlist?list=PL-osiE80TeTvipOqomVEeZ1HRrcEvtZB_)

### 兩大觀念
1. **plt** 
  - import後就可以直接用，如果只要畫一張圖，用plt就夠了
  - 只是一個畫圖的函式，看不出實際上的意義
2. **ax**
  - 如果要畫兩張以上的圖用ax
  - 功能比plt多
  - ax有實際上的意義(圖上的物件)

![概念圖](https://github.com/writeforfun/matplotlib-selfstudy/blob/master/concept.png)

看上面的概念圖可以得知:
- fig = Figure
  - fig就是整張畫布
- ax = Axes ( ax != Axis)
  - ax是畫布上的圖， **~~不是軸~~**
  
定義ax的兩種方法 (fig用不到，但就是會回傳所以必須定義):

1. 
```python
fig, ax = plt.subplots() #ax = plt
```
2.
```python
fig = plt.figure()
# ax = plt.subplot(111)
ax = plt.subplot()
```
