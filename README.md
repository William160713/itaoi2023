# 網站內容講解
### 主要要注意的是html跟style.css這兩個檔案，相關的照片是放在images/下面

首頁是index.html，上面的menupage分別應對每個中文，
如果有需要就把名字改掉  

要注意的是如果改動上方的任何一個分頁，則其他的網頁也需要跟著更動。  

文字那些排版我主要都是用表格，相對比較簡單，有需要的話參考我的自己新增就可以。

#### html網頁內容

- 首頁
- 大會組織
	- 清單子項目
- 大會議程
	- 大會議程一覽表
- 專題演講
- 徵求論文
- 成果展報名
- 論文審查結果
- 研討會註冊
- 國家科技及技術委員會成果展
- 更多結果
	- 亞洲大學
	- 宜蘭大學
	- 雲端學會
	- wasn2022

我把大部分的內容都註解起來了，像是下面這些部分:

```
		<!--
		<section class="whyUs-section">
			<div class="container">
				
				<div class="featured-points">
					<ul>
						<li><i class="fas fa-book"></i> free books for students</li>
						<li><i class="fas fa-money-check-alt"></i> affordable fees</li>
						<li><i class="fas fa-chalkboard-teacher"></i> experienced teachers</li>
						<li> <i class="fas fa-book"></i> free books for students</li>
					</ul>
				</div>
				
				<div class="whyus-wrap">
					<h1>關於MC2022</h1> 
				</div>
			</div>
		</section>
		-->	

```

遇到這種的基本上可以不要理他，但是未來有需要的話就用`ctrl+ /` 的快捷鍵去掉註解
就可以再前面的網頁顯示出結果了。

***

#### css部分

css的部份的話主要是用來控制網頁元素的一些變化，比方說圖片放大縮小，  

如果menu一旦修改內容的話，裡面的字都需要新的排版，因此就需要更動`style.css`的內容(下方)



```
.menu-parent::after {
	content: "";
	border: solid #3a3a3a;
  	border-width: 0 3px 3px 0;
  	display: inline-block;
  	padding: 3px;
  	/* 修改上方導航間距 */
	margin-left: 100px;
  	transform: rotate(45deg);
  	-webkit-transform: rotate(45deg);
}
```

只要直接搜尋margin-left的部分，把`100px`的地方數字依照看狀況調整大小就可以了

banner的大小要是要換的話，就是修改下方程式碼:

```
.banner img {
	/*banner 照片的設計 調整長寬都放在這*/ 
	opacity: 0.5; 
    filter: alpha(opacity=50); 
	height: 600px;
	width: 100%;
}
```

其中`opacity: 0.5; `的地方設置為1的話就會是完全清晰，往下設置就會模糊  

`	height: 600px;
	width: 100%;`  的部分修改長寬的結果。


	
> 可以參考的網站: https://www.w3schools.com/tags/default.asp
