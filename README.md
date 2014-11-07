
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
   <head>
   <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
         <title>Form with ul</title>
		 <style type="text/css">
		 ul {
		 list-style-type: none;
		 padding-left: 0;
		 }
		 fieldset {
		 margin-top: 20px;
		 }
		 .changed li {
	     padding-top: 10px;
         }
		 .standard li {
		 padding-top: 0;
		 }
		 .hint {
		 color: #696969;
		 font-family: Verdana;
		 }
		 .hint:focus {
		 color: #000000;
		 }
		 </style>
   </head>
   <body>
      <form action="111" method="post">
         <fieldset>
		 <legend><b>Коротко о себе</b></legend>
		    <ul class="changed li">
			   <li><label>Имя: <input type="text" name="first_name" size="30" maxlength="20" /></label></li>
			   <li><label>Фамилия: <input type="text" name="second_name" size="30" maxlength="30" /></label></li>
			   <li>Пол: <input type="radio" name="sex" id="man" value="male" checked="checked" /><label for="man">мужской</label> 
			            <input type="radio" name="sex" id="vomen" value="female" /><label for="vomen">женский</label></li>
		       <li><label>Возраст: <input type="text" name="age" size="5" /> лет</label></li>
			</ul>
		 </fieldset>
		 <fieldset>
		 <legend><b>Подробнее о себе</b></legend>
		    <ul class="changed li">
			   <li>
			      <ul class="standard li">
				     <li><input type="radio" name="gender" id="boy" value="g1" checked="checked" /><label for="boy">Молодой человек</label></li>
			         <li><input type="radio" name="gender" id="girl" value="g2" /><label for="girl">Девушка</label></li>
				     <li><input type="text" name="birthday" id="birthday" /><label for="birthday"> Дата рождения</label></li>
                     <li><input type="text" name="family_status" id="fstatus" /><label for="fstatus"> Семейное положение</label></li>
			         <li><input type="text" name="social_status" id="sstatus" /><label for="sstatus"> Социальный статус</label></li>
			         <li><input type="text" name="residence" id="residence" /><label for="residence"> Местожительство</label></li>
				  </ul>
			   </li>
			   <li><p><b>Что вы обычно делаете на выходных:</b></p>
			      <ul class="standard li">
				     <li><input type="checkbox" name="weekend" id="us1" value="u1" /><label for="us1"> Сплю</label></li>
			         <li><input type="checkbox" name="weekend" id="us2" value="u2" /><label for="us2"> Гуляю с друзьями</label></li>
			         <li><input type="checkbox" name="weekend" id="us3" value="u3" /><label for="us3"> Хожу на рыбалку</label></li>
			         <li><input type="checkbox" name="weekend" id="us4" value="u4" /><label for="us4"> Играю в игры</label></li>
				  </ul>
			   </li>
			   <li><p><b>Рассказать о формах в книге, посвящённой HTML:</b></p>
			      <p><select size="1" name="form_book">
			      <option value="data1">Site frequency:</option>
			      <option value="data2">Site frequency 2:</option>
			      <option value="data3">Site frequency 3:</option>
			      </select></p>
			   </li>
			   <li><p><b>Сколько книг вы прочитали за свою жизнь:</b></p>
			      <ul class="standard li">
				     <li><input type="radio" name="books" id="ten" value="10" /><label for="ten"> 0-10</label></li>
			         <li><input type="radio" name="books" id="twenty" value="20" /><label for="twenty"> 11-20</label></li>
			         <li><input type="radio" name="books" id="fifty" value="50" /><label for="fifty"> 21-50</label></li>
			         <li><input type="radio" name="books" id="fiftypl" value="50+" /><label for="fiftypl"> 50+</label></li>
				  </ul>
			   </li>
			   <li><label for="comment"><b>Ваши комментарии:</b></label><br />
			      <textarea name="comment" id="comment" rows="6" cols="40"></textarea>
			   </li>
			   <li><select size="3" multiple="multiple" name="position">
			      <option value="pos1">Первая позиция</option>
			      <option value="pos2" selected="selected">Вторая позиция</option>
			      <option value="pos3">Третья позиция</option>
				  <option value="pos4">Четвёртая позиция</option></select>
			   </li>
			</ul>
		 </fieldset>
		 <fieldset>
		 <legend><b>И в заключении</b></legend>
                  <p><input type="text" size="40" name="unknown" class="hint" value="Это поле было введено до   вас" onfocus="this.value=''" onblur="this.value='Это поле было введено до вас'" /></p>
                  <p><label for="email"><b>Email:</b></label><br />
			      <input type="text" size="40" name="email" id="email" /></p>
            <ul class="changed li">
			   <li><p><b>Хотите подписаться на самую модную рассылку спама?</b><br />
			      <i>Выберите категории</i></p>
			      <ul class="standard li">
			         <li><label><input type="checkbox" name="category" value="equipment" /> Оборудование</label></li>
			         <li><label><input type="checkbox" name="category" value="lunch" /> Как приготовить обеды</label></li>
			         <li><label><input type="checkbox" name="category" value="million" /> Заработай миллион за два дня!</label></li>
			      </ul>
			   </li>
			   <li><p><b>На сколько сложная задача:</b></p>
			      <ul class="standard li">
			         <li><label><input type="radio" name="problem" value="nprob" checked="checked" /> Совсем нет</label></li>
			         <li><label><input type="radio" name="problem" value="norm" /> Так себе</label></li>
			         <li><label><input type="radio" name="problem" value="yprob" /> Еле справились</label></li>
			      </ul>
			   </li>
			</ul>
		 </fieldset>
		 <p><button type="submit" value="sub">Отправить</button></p>
      </form>
   </body>
</html>

