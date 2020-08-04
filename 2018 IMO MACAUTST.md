# 2018 IMO MACTST

**Problem 5.** $在銳角$ $\triangle ABC\ (AC \neq BC)$$，已知$ $AE \perp BC\ $$於點$ $E、$$BF \perp AC$ 於點 $F$$。設圓$ $\Gamma$ $通過$ $E$、$F$ $且與$ $AB$ $邊相切於$ $D$ $點，$$並有$ $[\triangle ADE] = [\triangle BDF]$$。證明$ $\angle EDF = \angle ACB$

**Analysis.** $這道題所給出的已知條件十分簡單，$$看似是一道題初三至高一難度的幾何題。$$實質上，這道題才是真正的\ ``\ 扮豬食老虎"，$$足以難倒近九成的高中生，不然怎會成為\ 2018\ 年澳門區\ \text{IMO}\ 選拔賽難題。$$不過，無論題目多麼難，它始終都是可解的，$$且解法都是利用常規套路。$$今次，筆者便介紹其中一種常規思路\ (筆者常用)，對幾何仍有恐懼的讀者可以不妨嘗試接納。$
$$
\fbox{$\text{角分析 Angle Chasing}\ \rightarrow\ \text{邊分析 Length Chasing}\ + \text{面積分析 Area Chasing}\rightarrow \text{三角分析 Trigonometric Analysis}$} 
$$
$同時，筆者給出兩個解答，一長一短，短解答沒有使用\ \text{Trigonometric Analysis}，長解答有，讀者可以不妨參詳一下。$

**Proof & Tutorial.**

<img src="2018_IMOTSTP5.png" alt="2018_IMOTSTP5" style="zoom:20%"/>

- $1.\ \text{Angle Chasing:}$

	$一開始，我們只能嘗試找切入點，用你的直覺和知識，盡量找出角與角之間的關係。無論到最後有沒有用，都請你一一記下。$
	$\text{Angle Chasing}\ 的重要手段有四，其一是\textbf{四點共圓}，其二是\textbf{平行關係}，其三是\textbf{相似三角形}，另一是\textbf{把剩下的角都試一遍}。$	

	- $1.1\ \text{四點共圓}$
		$因為\ \angle AFB = \angle AEB = 90^{\circ}，所以\ A、F、E、B\ 四點共圓。$$所以\ \angle EFC = \angle ABC\ 且\ \angle FEC = \angle BAC。$
		$因為\ \angle HEC = \angle HFC = 90^{\circ}，所以\ H、F、C、E\ 四點共圓。$$所以\ \angle BHE = \angle AHF = \angle ACB。$

		
	
	- $1.2\ 平行關係$
		$找遍了整幅幾何圖\ (未畫點\ M、N、H)，都未能找到平行關係。$
	
	
	
	- $1.3\ 相似三角形$
		$由\ 1.1\ 的結論可知，\triangle CEF \sim \triangle CAB。$
	
		
		
	- $1.4\ 試剩下的角一遍$	
	$\angle BDE = \angle DFE，\angle ADF = \angle DEF\ (弦切角定理)$	
	$\angle DEB = 180^{\circ} - \angle BDE - \angle DBE = 180^{\circ} - \angle DFE - \angle EFC = 180^{\circ} - \angle DFC = \angle DFA\ (*)$
	
---

​		$注意，1.1$ ~ $1.3$ $的特點都與\ D\ 點沒有關係，即使用其他三角形\ \triangle A'B'C' 來取代\ \triangle ABC，這三個結論依然成立。$
​		$但是，\angle DEB = \angle DFA\ 的特點可不是隨便一個三角形就能滿足。每當出現這種\ ``\ 奇異點"，大多數都意味着\ ``\ 切入點"的浮現。$
​		$此時，如果結論\ ``\angle EDF = \angle ACB" 成立，那麼必定有\ ``四邊形\ DECF\ 是平行四邊形" 的結論。$	
​		$倒過來想，如果有\ ``四邊形\ DECF\ 是平行四邊形" 的結論成立，那麼結論\ ``\angle EDF = \angle ACB" 也成立。$	
​		$所以，結論\ ``\angle EDF = \angle ACB" 成立等價於\ ``四邊形\ DECF\ 是平行四邊形" 成立。\hspace{6em}{\fbox{等價變換}}$

​		$由初二學過的幾何知識可知，``四邊形\ DECF\ 是平行四邊形" 成立等價於\ ``DE \parallel CF\ 且\ EC \parallel FD" 成立。$	
​		$由初一學過的幾何知識可知，``DE \parallel CF" 成立等價於\ ``\angle EDF = \angle DFA"成立。$	
​		$而\ \angle DFA = \angle DEB\ 一直成立，所以又等價於\ ``\angle DEB = \angle EDF" 的成立。$
​		$同時，``\angle DEB = \angle EDF" 的成立等價於\ ``EC \parallel FD" 成立。$
​		$綜上所述，``DE \parallel CF" 成立等價於\ ``EC \parallel FD" 成立。因此，``四邊形\ DECF\ 是平行四邊形" 成立等價於\ ``EC \parallel FD" 成立。$

---

- $2(Short). \text{Length Chasing + Area Chasing}$

	$利用\ [\triangle ADE] = [\triangle BDF]\ 同時進行兩項\ \text{Chasing}:$
	$$
	[\triangle ADE] = [\triangle BDF]
	$$
	$$
	\frac{1}{2}DE \cdot AE \cdot \sin \angle DEA= \frac{1}{2}DF \cdot BF \cdot \sin \angle BFD
	$$
	$$
	DE \cdot AE \cdot \cos\angle DEB = DF \cdot BF \cdot \cos \angle DFA
	$$
	$$
	DE \cdot AE = DF \cdot BF
	$$
	$$
	\frac{DE}{DF} = \frac{BF}{AE} = \frac{CA \cdot BF}{CB \cdot BF} \cdot \frac{CB}{CA} = \frac{2[\triangle ABC]}{2[\triangle ABC]} \cdot \frac{CB}{CA} = \frac{CB}{CA} \tag{1}
	$$
	$因為\ \triangle CEF \sim \triangle CAB，所以$
	$$
	\frac{CF}{CE} = \frac{CB}{CA} = \frac{DE}{DF}
	$$
	$$
	DE \cdot CE = DF \cdot CF \tag{2}
	$$
	$$
	[\triangle DEC] = \frac{1}{2}DE \cdot CE \cdot \sin\angle DEC = \frac{1}{2}DF \cdot CF \cdot \sin\angle DFA = [\triangle DFC] \tag{3}
	$$
	$以\ CD\ 為底邊，結合\ (3)\ 式可得$
	$$
	\frac{1}{2}CD \times (\text{$E\ 到\ CD\ 的距離$}) = \frac{1}{2}CD \times (\text{$F\ 到\ CD\ 的距離$})
	$$
	$$
	\text{$E\ 到\ CD\ 的距離$} = \text{$F\ 到\ CD\ 的距離$}
	$$
	
	$接下來，我們試着作\ E\ 點關於\ CD\ 的對稱點\ E':$
	$此處有$
	$$
	\angle DE'C = \angle DEC = \angle DFC\ \Leftrightarrow D、E'、F、C\ \text{四點共圓} \tag{4}
	$$
	$同時也有$
	$$
	\text{$E'\ 到\ CD\ 的距離$} = \text{$E\ 到\ CD\ 的距離$} = \text{$F\ 到\ CD\ 的距離$}
	$$
	$所以有\ E'F \parallel CD。$
	$利用\ ``如果圓內接四邊形存在一組對邊平行，那麼這個四邊形只能是矩形或等腰梯形" 這個定理，可得$
	$$
	\angle FDC = \angle E'CD = \angle ECD\ \Leftrightarrow EC \parallel FD
	$$
	
	
	
	$相信有很多讀者都認為自己已經可以獲得滿分，但，其實上述的證明是有一個小缺陷的。$
	$那就是\ ``E'\ 和\ F\ 是否會重合" 的問題，大家不妨想像一下\ ``箏形"。$
	$如果\ DFEC\ 是箏形，那麼它依然滿足\ \angle DEB = \angle DFA\ 和\ [\triangle DEC] = [\triangle DFC]\ 這兩個條件，但，\angle EDF \neq \angle ACB，出事。$
	
	
	
	$要證明\ ``E'\ 和\ F\ 不會重合"，只需證明\ ``CE \neq CF" 便可。$
	$因為\ \frac{CE}{CF} = \frac{CA}{CB}，所以\ ``CE \neq CF" 等價於\ ``CA \neq CB"。$
	$因為\ AC \neq BC，所以\ E'\ 和\ F\ 不會重合，證明修復成功。$
---

- $2(Long).\ \text{Length Chasing + Area Chasing}$

	$接續\ 1，可以發現\ \text{Angle Chasing}\ 已經發揮得七七八八，是時候要進入\ \text{Length Chasing + Area Chasing}\ 的部分。$
	$既然在幾何圖上看到了這麼多的切線和割線，我相信讀者們應該不難想到接下來要用到\ ``圓冪定理"。$

	$記\ AE、BF\ 分別交圓\ \Gamma\ 於點\ M、N，AE\ 交\ HF\ 於點\ H\ (垂心)。$
	$由圓冪定理知$
	$$
	\frac{BH}{AH} = \frac{EH}{FH} = \frac{NH}{MH}
	$$
	$所以會得出\ MN \parallel AB，由此可推得$
	$$
	\frac{[\triangle ADM]}{[\triangle BDN]} = \frac{AD}{BD} \tag{1}
	$$
	$但是點\ M、N\ 始終是輔助點，我們希望能夠消去這兩點。$
	
	$利用\ \text{Area Chasing}\ 可得$
	$$
\frac{[\triangle ADM]}{[\triangle ADE]} = \frac{AM}{AE} = \frac{AM \cdot AE}{AE^2} = \frac{AD^2}{AE^2} \tag{2}
	$$
	$$
\frac{[\triangle BDN]}{[\triangle BDF]} = \frac{BN}{BF} = \frac{BN \cdot BF}{BF^2} = \frac{BD^2}{BF^2} \tag{3}
	$$

	$兩式相除可得$
	$$
	\frac{(2)}{(3)} := \frac{[\triangle ADM]}{[\triangle BDN]} = (\frac{AD}{BD})^2 \cdot (\frac{BF}{AE})^2
	$$
	$結合\ (1)\ 式可得$
	$$
	\frac{AD}{BD} = (\frac{AD}{BD})^2 \cdot (\frac{BF}{AE})^2
	$$
	$$
	\Leftrightarrow \frac{AD}{BD} = (\frac{AE}{BF})^2 \tag{3}
	$$
	$到此，我們達成了消去\ M、N\ 的目標。$
	
	$注意到，AE、BF\ 都是\ \triangle ABC\ 邊上的高，所以這些線段都可以用\ \triangle ABC\ 的邊和角表示出來。$	
	$因為$
	$$
	\frac{1}{2}CB \times AE = [\triangle ABC] = \frac{1}{2}CA \times BF
	$$
	$所以$
	$$
	\frac{AE}{BF} = \frac{CA}{CB} \tag{4}
	$$
	$結合\ (3)\ 式可得$
	$$
	\frac{AD}{BD} = (\frac{CA}{CB})^2 \tag{5}
	$$
	
	$既然\ AD、BD\ 都是切線長，怎可能少得了\ ``切線長定理"$	
	$令\ (5)\ 式進行平方，可得$
	$$
	(\frac{CA}{CB})^4 = \frac{AD^2}{BD^2} = \frac{AM}{BN} \times \frac{AE}{BF} = \frac{AH}{BH} \times \frac{CA}{CB} = \frac{AF}{BE} \times \frac{CA}{CB}
	$$
	$$
		\Rightarrow \frac{AF}{BE} = (\frac{CA}{CB})^3 \tag{6}
	$$
	
	$下面，我們試着把一些線段用邊\ AB、BC、CA\ 表示出來:$	
	$由\ (4)\ 式可得$
	$$
		AE^2 = (\frac{CA}{CB})^2BF^2 \tag{7}
	$$
	$由\ (6)\ 式可得$
	$$
        BE^2 = (\frac{CB}{CA})^6FA^2 \tag{8}
	$$
	$對直角\ \triangle BEA\ 和\ \triangle BFA\ 使用勾股定理:$
	$$
		AB^2 = AE^2 + BE^2 = (\frac{CA}{CB})^2BF^2 + (\frac{CB}{CA})^6FA^2 \tag{9}
	$$
	$可以分別算得$
	$$
		BF^2 = \frac{1 - (\frac{CB}{CA})^6}{(\frac{CA}{CB})^2 - (\frac{CB}{CA})^6} AB^2 = \frac{CB^6 - CA^6}{CB^8 - CA^8} \cdot CB^2 \cdot AB^2\tag{10}
	$$
	$$
	FA^2 = \frac{1 - (\frac{CA}{CB})^2}{(\frac{CB}{CA})^6 - (\frac{CA}{CB})^2} AB^2 = \frac{CB^2 - CA^2}{CB^8 - CA^8} \cdot CA^6 \cdot AB^2 \tag{11}
	$$
---

- $3(Long).\ \text{Trigonometric Analysis}$ 

	$接下來，所有的邊長分析，都會轉變成三角分析:$
	- $3.1\ (10)\ 式變換:$
		$注意到$
		$$
			\sin \angle ACB = \frac{BF}{CB}
		$$
		$再結合正弦定律，可得$
		$$
		\frac{\sin^6 A - \sin^6 B}{\sin^8 A - \sin^8 B} = 1\ \Leftrightarrow \frac{\sin^4 A + \sin^4 B + \sin^2 A\sin^2 B}{(\sin^2 A + \sin^2 B)(\sin^4 A + \sin^4 B)} = 1 \tag{12}
		$$

	- $3.2\ 計算 \frac{AD}{AF}:$
		$由\ (5)\ 式可得$
		$$
			AD = \frac{CA^2}{CA^2 + CB^2} \cdot AB \Leftrightarrow AD^2 = \frac{CA^4}{(CA^2 + CB^2)^2} \cdot AB^2 \tag{13}
		$$
		$結合\ (11)\ 式可知$
		$$
			(\frac{AD}{AF})^2 = \frac{CA^4 + CB^4}{CA^2 \cdot (CA^2 + CB^2)} \tag{14}
		$$
		$要證明\ ``EC \parallel FD" 成立，則等價於證明\ ``\frac{AD}{AF} = \frac{AB}{AC}"$
		$因此等價於證明$
		$$
		(\frac{AD}{AF})^2 = \frac{CA^4 + CB^4}{CA^2 \cdot (CA^2 + CB^2)} = (\frac{AB}{AC})^2
		$$
		$$
			\Leftrightarrow \frac{CA^4 + CB^4}{CA^2 + CB^2} = AB^2
		$$
		$利用餘弦定律可得\ AB^2 = CA^2 + CB^2 - 2CA \cdot CB \cos C$
		$即等價於$
		$$
			\Leftrightarrow CA^4 + CB^4 = (CA^2 + CB^2)(CA^2 + CB^2 - 2CA \cdot CB \cos C)
		$$

		$$
			\Leftrightarrow CA^4 + CB^2 = CA^4 + CB^4 + 2CA\cdot CB \cdot [CA \cdot CB - (CA^2 + CB^2)\cdot \cos C]
		$$
		$$
			\Leftrightarrow \frac{CA \cdot CB}{CA^2 + CB^2} = \cos C
		$$
		$再次利用正弦定律可得$
		$$
			\Leftrightarrow \frac{\sin A \cdot \sin B}{\sin^2 A + \sin^2 B} = -\cos(A + B) = \sin A \sin B - \cos A \cos B
		$$
		$$
			\Leftrightarrow \sin A \sin B \cdot (1 - \frac{1}{\sin^2 A + \sin^2 B}) = \cos A \cos B \tag{15}
		$$
		$下一步當然是希望左右兩式進行平方，但是我們要說明平方式與原式等價:$
		$因為\ \triangle ABC\ 銳角三角形，所以\ \cos A > 0\ 且\ \cos B > 0，因此\ (15)\ 式的右式大於\ 0。$
		$關於\ (15)\ 式的左式，我們要利用\ (12)\ 式的恆等變換:$ 
		$$
			(12) \Leftrightarrow \sin^2 A + \sin^2 B = 1 + \frac{\sin^2 A \sin^2 B}{\sin^4 A + \sin^4 B} > 1
    $$
		$所以\ (15)\ 式的左式也是大於\ 0。$
		$由此可得$
		$$
		(15) \Leftrightarrow \sin^2 A \sin^2 B \cdot (1 - \frac{1}{\sin^2 A + \sin^2 B})^2 = \cos^2 A \cos^2 B = (1 - \sin^2 A)(1 - \sin^2 B)
		$$
		$$
			\Leftrightarrow \frac{\sin^2 A \sin^2 B}{(\sin^2 A + \sin^2 B)^2} - \frac{2\sin^2 A \sin^2 B}{\sin^2 A + \sin^2 B} = 1 - \sin^2 A - \sin^2 B
		$$
		$$
			\Leftrightarrow 1 = \frac{\sin^2 A \sin^2 B}{(\sin^2 A + \sin^2 B)^2} + \sin^2 A + \sin^2 B - \frac{2\sin^2 A \sin^2 B}{\sin^2 A + \sin^2 B}
		$$
		$$
			\Leftrightarrow 1 = \frac{\sin^2 A \sin^2 B}{(\sin^2 A + \sin^2 B)^2} + \frac{\sin^4 A + \sin^4 B}{\sin^2 A + \sin^2 B}
		$$
		$$
			\Leftrightarrow 1 = \frac{\sin^2 A \sin^2 B}{(\sin^2 A + \sin^2 B)^2} + \frac{(\sin^2 A + \sin^2 B)(\sin^4 A + \sin^4 B)}{(\sin^2 A + \sin^2 B)^2} \tag{16}
		$$
		$再次利用\ (12)\ 式:$
		$$
			(12) \Leftrightarrow (\sin^2 A + \sin^2 B)(\sin^4 A + \sin^4 B) = \sin^4 A + \sin^4 B + \sin^2 A\sin^2 B \tag{17}
		$$
		$所以$
		$$
		(16) \Leftrightarrow 1 = \frac{\sin^2 A \sin^2 B}{(\sin^2 A + \sin^2 B)^2} + \frac{\sin^4 A + \sin^4 B + \sin^2 A\sin^2 B}{(\sin^2 A + \sin^2 B)^2} = \frac{(\sin^2 A + \sin^2 B)^2}{(\sin^2 A + \sin^2 B)^2} = 1
		$$
$由於以上每步皆可逆，所以\ ``\frac{AD}{AF} = \frac{AB}{AC}" 成立$。
