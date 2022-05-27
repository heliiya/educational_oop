با سلام
در این بخش می خواهم مفهوم شی گرایی را در قالب یک پروژه توضیح دهم:
پروژه تعریف شده به این صورت است که اشکال مختلف را به عنوان ورودی گرفته و محیط و مساحت و تعداد اضلاع و شعاع داخلی و شعاع خارجی آنها را محاسبه می کند.
Object-Oriented Programming:
1. Abstraction:
در این مرحله ما تصمیم گرفتیم که پروژه را به صورت زیر پیاده سازی کنیم:
(abstract superClass) Shape  
	----> (subClass) Oval  ----> (subClass) Circle
	----> (subClass) Parallelogram  
			----> (subClass) Rectangle implements RectangleLike
			----> (subClass) Rhombus implements RhombusLike
			---->(subClass)Square implements RectangleLike,RhombusLike
	 ----> (abstract superClass) RegularPolygon 
			----> (subClass) RegularHeptagon
			----> (subClass) RegularHexagon
			----> (subClass) RegularPentagon
	----> (subClass) Trapezoid
	----> (subClass) Triangle
و محیط و مساحت و تعداد اضلاع و شعاع داخلی و شعاع خارجی  را که در مختص به شکل بودن است و ربطی به اینکه چه شکلی می باشد ندارد، را در سوپرکلاس    تعریف می کنیم. Shape 
2. Inheritnace:
پیاده سازی انجام شده در مرحله قبل باتوجه به وجود ویژگی ارث بری می باشد. به این صورت که ساب کلاس ها، توابع سوپرکلاس را به ارث برده و می توانند آنها را مطابق با کلاس خودشان تغییر دهند.
3. Polymorphism:
با توجه به این ویژگی سوپرکلاس شیپ می تواند به ریخت تمام اشکال موجود در بیاید و هرکدام از شکل ها، متدهای آن را به صورتی که خودشان می خواهند پیاده سازی کنند.
4. Encapsulation:
برای رعایت این اصل در پروژه، تمام متغیرهای هر کلاس را به صورت پرایویت تعریف کرده و با استفاده از
آنها بهشان دسترسی داریم. getter , setter
و اینکه بدنه ی متدهایی که در بخش سوم شی گرایی گفتیم که در هر کلاس به صورت جداگانه پیاده سازی  می کنیم، تنها مختص همان کلاس می باشد.
