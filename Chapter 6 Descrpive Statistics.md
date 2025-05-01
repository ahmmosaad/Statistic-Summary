اﻹحصاء بشكل عام وظيفتها توصفلي وتلخصلي الداتا في شوية أرقام وممكن ألخص الداتا بكذا طريقة:
1. Frequancy Table
2. Numerical Summary
3. Graphs

## The Sample
بس قبل منبدأ في الحاجات دي في شوية حاجات مهم إننا نعرفها عن الداتا الي هنشتغل فيها 
Population: all elements posess the charactrstics of interest
بروح أخد منها عينة
Sample: portion of population
وممكن العينة دي تكون فيها إنحياز أو ﻻ والي فيها واﻹنحياز نوعين
Convenience biased sample هنا مبذلتش مجهود في اﻹختيار 
Voluntery response biased sample وهنا الناس المتطوعين هما الي اختارو

طيب ازاي اخد عينة مفيهاش إنحياز؟ باتباع اخد الطرق اﻵتية
1- Simple random sampling
كل العناصر ليها نفس الفرصة إنها يتم أختيارها
2- Stratified Random Sampling
بقسمهم مجموعات حسب التشابه بينهم وبعدين اختار من كل مجموعة عشوائي
3- Clustering Sampleing
بقسمهم مجموعات عشوائية متساويى وبعدين أختار عشوائي من كل مجموعة

## Data Types
1. Quantitative
	- numerical
		- Discrete: finite or countably infinte of numer
		- Continuous: take value in an interval number
2. Qualitative: non numerical value (nominal) like color, gender ..etc
3. Logical: true or false
4. Missing
5. Other

## Numerical Summary

> 1. Measures Centerlity or Center tendancy or Location
> 	- Mean
> 	- Median
> 		
> 	- mode
> 	- trimmed mean
> 	- weighted mean
> 2. Measure of variability - spread - dispersion
> 	- Range
> 	- variance
> 	- standard devision
> 3. Measure of shape 
> 	- skwness: right - left - symetric
> 	- Kurtosis: light - heavy
> 4. Measure of relative Position 
> 	- Percentile 
> 	- quartiles
> 	- IQR
> 	- Coefficent of variation
> 5. Graph and diagram
> 	- stem and leaf diagram
> 	- Freaquency distributions and Histogram
> 	- Box plots
> 	- Time Sequance Plots
> 	- Probability Plots

**1- Mean**
دا متوسط اﻷرقام الي عندي، بجمعهم وأقسمهم على عددهم يديني المتوسط بتاعم، ودا بجيبة للـ Sample and Population
- Sample mean:
	$$\bar{x} = \frac{1}{n} \sum_{i=1}^{n} x_i$$
		- the average value of all of the observation.
		- 
		
- Population mean

وخلي بالك دا بيتأثر جدا بالـOutliers ودي عبارة عن القيم الشاذة المختلف عن باقي القيم ممكن تكون كبيرة جدا أو صغيرة جداً
3- Median
هنا أنا برتبهم وأجيب القيمة الي في النص بالظبط طبعا هتختلف لو عدد زوجي أو فردي ودا القانون بتاعها
$$ \text{Median}(X) = 
\begin{cases}
x_{\left(\frac{n+1}{2}\right)} & \text{if } n \text{ is odd,} \\
\frac{x_{\left(\frac{n}{2}\right)} + x_{\left(\frac{n}{2}+1\right)}}{2} & \text{if } n \text{ is even.}
\end{cases}$$
ومبيتأثرش بالـOutliers قوي زي المتوسط
4- Trimmed mean
علشان أتغلب على تأثير القيم الشاذة ممكن ألجا أني أستبعد جزء معين من الداتا، ممكن مثلا أكبر وأصغر ١٠% من الداتا بتعتي 

$$ \bar{x}_{\text{trim}} = \frac{1}{n} \sum_{i=1}^{n} x_{(i)}$$

5- Weighted mean



### Measure of variability - spread - dispersion

1- Range
ودا الفرق بين أكبر قيمة وأقل قيمة في الداتا الي معايا
$$\text{Range} = \max(x_i) - \min(x_i)$$

2- variance
دا فكرته اني بجيب الفرق بين كل نقطة وبين الـMean الفرق دا بيبينلي مقدار تشتتت وابتعاد القيم عن بعضها. ف النقط الي أكبر من المتوسط هتطلع موجب واﻷقل هتطلع سالب ومجموعهم في اﻵخر صفر. علشان نتجنب حوار الصفر دا عن طريق إننا نربع الفرق بين القيمتين دول.
فقولنا نعمل قانون يطلع رقم معين يعبر عن مقدار التشتت دا فطلعنا بالـVariance وبيجي بالقانون دا:
Population

		$\sigma^2 = \frac{1}{N} \sum_{i=1}^{N} (X_i - \mu)^2$

Sample

		$s^2 = \frac{1}{n-1} \sum_{i=1}^{n} (x_i - \bar{x})^2$
	

المقام هنا (n-1) ليه اسم تاني Degree of freedom ليه؟
علشان القيم دي لو مسكت كل قيمة طرحتها من المتوسط، وجمعت القيم هتطلع بيساوي صفر، فلو عندي كل القيم ماعدا واحدة أقدر اجيبها بالطريقة دي لو معايا المتوسط.
![[f72c7b791614a4cda9503fe1c1749ddca.jpg| 300]]
طيب ليه (n-1) ؟
علشان بنسبة كبيرة صعب تجيب متوسط بتاع الـPopulation فبجيب فبستخدم غالبا متوسط العينة، وكمان قيمة الـXi غالبا بتكون أقرب لمتوسط العينة من متوسط التاني، لذلك بيقسم على القيمة دي بدل الـn

3- standard devision
دا بقى بنجيبه ازاي؟ هو الجذر التربيعي للـVariance وبيجي بالقانون دا
Population
		$\sigma = \sqrt{\sigma^2} = \sqrt{\frac{1}{N} \sum_{i=1}^{N} (X_i - \mu)^2}$

Sample

		$s = \sqrt{s^2} = \sqrt{\frac{1}{n-1} \sum_{i=1}^{n} (x_i - \bar{x})^2}$
		

### Measure of shape 

 Skwness:
 indicates whether the data is concentrated more on one side of the mean compared to the other.
 شكل توزيع الداتا بتعتي بيكون عامل ازاي؟ هل هي 
**Negatively Skewed (Left-Skewed)**
The left tail is longer; the mass is concentrated on the right.
Mean < Median < Mode

**Positively Skewed (Right-Skewed)**
The distribution is balanced around the mean
Mean = Median = Mode

**Positively Skewed (Right-Skewed)**
The right tail is longer; the mass is concentrated on the left. 
Mean > Median > Mode
![[Capture_20250428_160128.jpg|300]]
وفي معادﻻت بتحسب الـSkewness Coffe
Population Skewness:
$\gamma_1 = \frac{\mu_3}{\sigma^3} = \frac{E[(X - \mu)^3]}{\sigma^3}$

Sample Skewness 
$g_1 = \frac{m_3}{s^3} = \frac{\frac{1}{n} \sum_{i=1}^n (x_i - \bar{x})^3}{\left( \sqrt{\frac{1}{n} \sum_{i=1}^n (x_i - \bar{x})^2} \right)^3}$

Adjusted Fisher-Pearson Skewness (for small samples)
$G_1 = \frac{\sqrt{n(n-1)}}{n-2} \cdot g_1$

بغض النظر عن اي قانون هتستخدمة من دول لو القيمة تساوي صفر فهو symertic لو أكبر right لو اقل من صفر يبقى شمال

ولو خدت القيمة المطلقة |skewness| وطلعت أقل من 0.5 يبقى التوزيع متثماثل
لو بين النص والواحد يبقى moderately skewed 
ولو أكبر من واحد يبقى highly skewed


 Kurtosis:
 دا بيشتغل على الـCurve tail وشكله وامتداده ومستوى ضيق واتساع المنحنى بيحاول يشوفي في اي اكستريم وﻻ ﻻ هي الديل مسحوب جامد زي اﻻسود وﻻ زي الازرق القيم تقريبا زي بعض 
 light - heavy
 
![[f5746015ac1bf47c2a83e8bfec92b66a5.jpg|300]]
![[f1b745a21c8ef4b87ba26b40c2e0bb6cc.jpg|100]]
وفي منه أنواع:
1. **Mesokurtic (Normal Kurtosis, )**  
   - Tails similar to a normal distribution (e.g., Gaussian distribution).  
   - Example: Standard normal distribution.

2. **Leptokurtic (High Kurtosis,)**  
   - Sharper peak and **fatter tails** (more outliers).  
   - Example: Financial returns (extreme gains/losses).

2. **Platykurtic (Low Kurtosis,)**  
   - Flatter peak and **thinner tails** (fewer outliers).  
   - Example: Uniform distribution.
![[Kurtosis1.webp]]

وفي معادﻻت بتحسب الـK

Population Kurtosis
$\beta_2 = \frac{\mu_4}{\sigma^4} = \frac{E[(X - \mu)^4]}{\sigma^4}$

 Sample Kurtosis
 $b_2 = \frac{m_4}{s^4} = \frac{\frac{1}{n} \sum_{i=1}^n (x_i - \bar{x})^4}{\left( \sqrt{\frac{1}{n} \sum_{i=1}^n (x_i - \bar{x})^2} \right)^4}$
 Excess Kurtosis
Since the normal distribution has kurtosis = 3, **excess kurtosis** is often used:

$g_2 = \beta_2 - 3 \quad \text{(Population)}$
$g_2 = b_2 - 3 \quad \text{(Sample)}$

- **Excess Kurtosis = 0** → Mesokurtic (normal tails).  
- **Excess Kurtosis > 0** → Leptokurtic (fat tails).  
- **Excess Kurtosis < 0** → Platykurtic (thin tails).  
### Measure of relative Position 

Percentile 
quartiles
IQR
Coefficent of variation