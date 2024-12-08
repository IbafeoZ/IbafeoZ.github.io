<script type="text/javascript" language="JavaScript">
 var res="1111111111" 
function check_me()
{
    var count=0
    with(document.test)
{
if (!Q1[0].checked&&!Q1[1].checked&&!Q1[2].checked&&!Q1[3].checked&&!Q1[4].checked)  
{count+=1};  
if (!Q2[0].checked&&!Q2[1].checked&&!Q2[2].checked&&!Q2[3].checked&&!Q2[4].checked)  
{count+=1};  
if (!Q3[0].checked&&!Q3[1].checked&&!Q3[2].checked&&!Q3[3].checked&&!Q3[4].checked)  
{count+=1};  
if (!Q4[0].checked&&!Q4[1].checked&&!Q4[2].checked&&!Q4[3].checked&&!Q4[4].checked)  
{count+=1};  
if (!Q5[0].checked&&!Q5[1].checked&&!Q5[2].checked&&!Q5[3].checked&&!Q5[4].checked)  
{count+=1};  
if (!Q6[0].checked&&!Q6[1].checked&&!Q6[2].checked&&!Q6[3].checked&&!Q6[4].checked)  
{count+=1};  
if (!Q7[0].checked&&!Q7[1].checked&&!Q7[2].checked&&!Q7[3].checked&&!Q7[4].checked)  
{count+=1};  
if (!Q8[0].checked&&!Q8[1].checked&&!Q8[2].checked&&!Q8[3].checked&&!Q8[4].checked)  
{count+=1};  
if (!Q9[0].checked&&!Q9[1].checked&&!Q9[2].checked&&!Q9[3].checked&&!Q9[4].checked)  
{count+=1};  
if (!Q10[0].checked&&!Q10[1].checked&&!Q10[2].checked&&!Q10[3].checked&&!Q10[4].checked)  
{count+=1};  
if (count>0) 
    {alert("Вы выполнили не все задания. Проверьте себя!")  } 
        else answer()
    }
} 
 
function control(k, f1,f2,f3,f4,f5,f6,f7,f8,f9,f10) {
if (k==1&&f1.checked) return true;
if (k==2&&f2.checked) return true;
if (k==3&&f3.checked) return true;
if (k==4&&f4.checked) return true;
if (k==5&&f5.checked) return true;
if (k==6&&f6.checked) return true;
if (k==7&&f7.checked) return true;
if (k==8&&f8.checked) return true;
if (k==9&&f9.checked) return true;
if (k==10&&f10.checked) return true;
return false;
}
 
function answer()
{
answ="";
     with(document)
    {
    answ+=control(res.charAt(0) ,test.Q1[0],test.Q1[1],test.Q1[2],test.Q1[3],test.Q1[4])?"1":"0"
answ+=control(res.charAt(1) ,test.Q2[0],test.Q2[1],test.Q2[2],test.Q2[3],test.Q2[4])?"1":"0"
answ+=control(res.charAt(2) ,test.Q3[0],test.Q3[1],test.Q3[2],test.Q3[3],test.Q3[4])?"1":"0"
answ+=control(res.charAt(3) ,test.Q4[0],test.Q4[1],test.Q4[2],test.Q4[3],test.Q4[4])?"1":"0"
answ+=control(res.charAt(4) ,test.Q5[0],test.Q5[1],test.Q5[2],test.Q5[3],test.Q5[4])?"1":"0"
answ+=control(res.charAt(5) ,test.Q6[0],test.Q6[1],test.Q6[2],test.Q6[3],test.Q6[4])?"1":"0"
answ+=control(res.charAt(6) ,test.Q7[0],test.Q7[1],test.Q7[2],test.Q7[3],test.Q7[4])?"1":"0"
answ+=control(res.charAt(7) ,test.Q8[0],test.Q8[1],test.Q8[2],test.Q8[3],test.Q8[4])?"1":"0"
answ+=control(res.charAt(8) ,test.Q9[0],test.Q9[1],test.Q9[2],test.Q9[3],test.Q9[4])?"1":"0"
answ+=control(res.charAt(9) ,test.Q10[0],test.Q10[1],test.Q10[2],test.Q10[3],test.Q10[4])?"1":"0"
 
showResult();
    }
}
 
function showResult()
{
    var nok=0;
    var i,s;
 
for (i=0; i<answ.length;i++) {nok+=answ.charAt(i)=="1"?1:0;}
if(nok==10) s="ОТЛИЧНО";
if(nok<10) s="ХОРОШО";
if(nok<7.5) s="УДОВЛЕТВОРИТЕЛЬНО";
if (nok<5) s="НЕУДОВЛЕТВОРИТЕЛЬНО";
    document.test.s1.
    value="Количество правильных ответов "+nok+". Ваша оценка  "+s+". Посмотрите на окно рядом с номером вопроса. Если ответ правильный, там (+). Если ответ ошибочен, там (-).";
 
with(document.test)
    {
    if (answ.charAt(0)=="1") {T1.value=" + "} else {T1.value=" - "};
   if (answ.charAt(1)=="1") {T2.value=" + "} else {T2.value=" - "};
   if (answ.charAt(2)=="1") {T3.value=" + "} else {T3.value=" - "};
   if (answ.charAt(3)=="1") {T4.value=" + "} else {T4.value=" - "};
   if (answ.charAt(4)=="1") {T5.value=" + "} else {T5.value=" - "};
   if (answ.charAt(5)=="1") {T6.value=" + "} else {T6.value=" - "};
   if (answ.charAt(6)=="1") {T7.value=" + "} else {T7.value=" - "};
   if (answ.charAt(7)=="1") {T8.value=" + "} else {T8.value=" - "};
   if (answ.charAt(8)=="1") {T9.value=" + "} else {T9.value=" - "};
   if (answ.charAt(9)=="1") {T10.value=" + "} else {T10.value=" - "};
     }
}
function showhide(obj){
    if(obj == 'none') return 'inline';
    else return 'none';
}
</script>
<center><b>Тест</b></center><br/><br/>
&nbsp;&nbsp;&nbsp;<span style="color:#006699;text-decoration:underline;cursor:pointer;" onclick="document.getElementById('instruction').style.display = showhide(document.getElementById('instruction').style.display)">
Инструкция</span>
 <br/>
<div id="instruction" style="display: none; width: 100%;">
<ul>
<li>Выберите один из вариантов в каждом из 10 вопросов;</li>
<li>Нажмите на кнопку "Показать результат";</li>
<li>Скрипт не покажет результат, пока Вы не ответите на все вопросы;</li>
<li>Загляните в окно рядом с номером задания. Если ответ правильный, то там (+). Если Вы ошиблись, там (-).</li>
<li>За каждый правильный ответ начисляется 1 балл;</li>
<li>Оценки: менее 5 баллов - НЕУДОВЛЕТВОРИТЕЛЬНО, от 5 но менее 7.5 - УДОВЛЕТВОРИТЕЛЬНО, 7.5 и менее 10 - ХОРОШО, 10 - ОТЛИЧНО;</li>
<li>Чтобы сбросить результат тестирования, нажать кнопку "Сбросить ответы";</li>
</ul>
</div>
<form name="test"><ol>
<li><INPUT type="text" size="1" name="T1"/><b> Какой этап изучения взаимосвязи живых организмов со средой описывается?</b><br/>
<input type="radio" name="Q1"/> Первый<br />
<input type="radio" name="Q1"/> Второй<br />
<input type="radio" name="Q1"/> Третий<br />
<input type="radio" name="Q1"/> Четвертый<br />
<input type="radio" name="Q1"/> Пятый<br />
<br/></li><li><INPUT type="text" size="1" name="T2"/><b> Что делали на втором этапе изучения взаимосвязи живых организмов со средой</b><br/>
<input type="radio" name="Q2"/> Накапливались данные<br />
<input type="radio" name="Q2"/> Делали научные обобщения<br />
<input type="radio" name="Q2"/> Оформляли результаты<br />
<input type="radio" name="Q2"/> Проводили эксперименты<br />
<input type="radio" name="Q2"/> Готовились к третьему этапу<br />
<br/></li><li><INPUT type="text" size="1" name="T3"/><b> На каком этапе делались первые научные обобщения?</b><br/>
<input type="radio" name="Q3"/> На первом<br />
<input type="radio" name="Q3"/> На втором<br />
<input type="radio" name="Q3"/> На третьем<br />
<input type="radio" name="Q3"/> На четвертом<br />
<input type="radio" name="Q3"/> На пятом<br />
<br/></li><li><INPUT type="text" size="1" name="T4"/><b> Что изучалось на первом этапе?</b><br/>
<input type="radio" name="Q4"/> Взаимосвязь живых организмов со средой<br />
<input type="radio" name="Q4"/> Данные о живых организмах<br />
<input type="radio" name="Q4"/> Научные эксперименты<br />
<input type="radio" name="Q4"/> Первые обобщения<br />
<input type="radio" name="Q4"/> Появление организмов<br />
<br/></li><li><INPUT type="text" size="1" name="T5"/><b> Какой характер был у данных на втором этапе?</b><br/>
<input type="radio" name="Q5"/> Количественный<br />
<input type="radio" name="Q5"/> Качественный<br />
<input type="radio" name="Q5"/> Смешанный<br />
<input type="radio" name="Q5"/> Неопределенный<br />
<input type="radio" name="Q5"/> Обобщенный<br />
<br/></li><li><INPUT type="text" size="1" name="T6"/><b> Какие первые обобщения делались на втором этапе?</b><br/>
<input type="radio" name="Q6"/> Научные<br />
<input type="radio" name="Q6"/> Эмпирические<br />
<input type="radio" name="Q6"/> Теоретические<br />
<input type="radio" name="Q6"/> Практические<br />
<input type="radio" name="Q6"/> Экспериментальными<br />
<br/></li><li><INPUT type="text" size="1" name="T7"/><b> Как называется процесс оформления результатов на втором этапе?</b><br/>
<input type="radio" name="Q7"/> Обобщение<br />
<input type="radio" name="Q7"/> Эксперимент<br />
<input type="radio" name="Q7"/> Классификация<br />
<input type="radio" name="Q7"/> Разработка<br />
<input type="radio" name="Q7"/> Изучение<br />
<br/></li><li><INPUT type="text" size="1" name="T8"/><b> Что делали на третьем этапе изучения взаимосвязи живых организмов со средой?</b><br/>
<input type="radio" name="Q8"/> Делали первые обобщения<br />
<input type="radio" name="Q8"/> Оформляли результаты<br />
<input type="radio" name="Q8"/> Накапливали данные<br />
<input type="radio" name="Q8"/> Проводили эксперименты<br />
<input type="radio" name="Q8"/> Изучали связь между организмами и средой<br />
<br/></li><li><INPUT type="text" size="1" name="T9"/><b> Какое значение имело взаимодействие живых организмов со средой на четвертом этапе</b><br/>
<input type="radio" name="Q9"/> Положительное<br />
<input type="radio" name="Q9"/> Отрицательное<br />
<input type="radio" name="Q9"/> Нейтральное<br />
<input type="radio" name="Q9"/> Разнонаправленное<br />
<input type="radio" name="Q9"/> Никакое<br />
<br/></li><li><INPUT type="text" size="1" name="T10"/><b> Какие научные выводы были сделаны на четвертом этапе изучения взаимосвязи живых</b><br/>
<input type="radio" name="Q10"/> Простые<br />
<input type="radio" name="Q10"/> Сложные<br />
<input type="radio" name="Q10"/> Системные<br />
<input type="radio" name="Q10"/> Индивидуальные<br />
<input type="radio" name="Q10"/> Вопросительные<br />
<br/></li></ol>     
<CENTER>
<P><TEXTAREA name="s1" rows="4" cols="70" readonly> </TEXTAREA> </P>
<INPUT onclick="check_me()" type="button" value="Показать результат"/>&nbsp;&nbsp;&nbsp;&nbsp; 
<INPUT type="reset" value="Сбросить ответы"/> 
</CENTER>        
</form> 
