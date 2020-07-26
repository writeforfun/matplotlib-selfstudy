# matplotlib-selfstudy
## The original tutorial can be found [here](https://www.youtube.com/playlist?list=PL-osiE80TeTvipOqomVEeZ1HRrcEvtZB)

### 兩大觀念
1. **plt** 是直接呼叫不用定義的，如果只要畫一張圖，用plt就夠了。
2. 如果要畫兩張以上的圖，就可以用 **ax**

![概念圖](https://github.com/writeforfun/matplotlib-selfstudy/blob/master/concept.png)

看上面的概念圖可以得知:
- fig = Figure
  - fig就是整張畫布
- ax = Axes ( ax =/= Axis)
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
