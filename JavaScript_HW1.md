| Task | JS code |
| --- | --- |
| 1. Создать переменную “item_1”<br>| let item_1;  |
| 2. Присвоить переменной item_1 цифру 5. | Item_1 = 5
| 3. Вывести в консоль item_1. |console.log(item_1)
| 4. Создать переменную “item_2”|let item_2;
| 5. Присвоить переменной item_2 цифру 3.|item_2 = 3;
|6. Вывести в консоль item_2.|console.log(item_2)
 |7. Создать переменную “item_3”|let item_3;
| 8. Присвоить переменной item_3 сложение item_1 и item_2.|item_3 = item_1 + item_2;
 |9. Вывести в консоль item_3.|console.log(item_3)
 |10. Создать переменную “item_4”|let item_4;
 |11. Присвоить переменной item_4 строку “Yolochka”|item_4 = "Yolochka"
 |12. Вывести в консоль item_4.|console.log(item_4)
 |13. Вывести в консоль сложение item_3 и item_4.|console.log(item_3 + item_4)
 |14. Вывести в консоль умножение item_3 и item_4.|console.log(item_3 * item_4)
 |15. Создать переменную “item_5”|let item_5;
 |16. Присвоить переменной item_5 переменную item_3|let item_5 = item_3;
 |17. Создать переменную item_6.|let item_6;
 |18. Создать переменную item_6_type|let item_6_type;
 |19. Присвоить переменной item_6 значение 15|item_6 = 15;
 |20. Присвоить переменной item_6_type тип переменной item_6|item_6_type = typeof item_6;
 |21. Вывести в консоль тип данных item_6 в виде ——  “item_6 == ”  item_6,  “item_6_type == ”  item_6_type ——  |console.log("item_6 ==", item_6, "item_6_type == ", item_6_type)
 |22. Создать переменную item_7 и в ней преобразовать item_6 в String.|let item_7; <br> item_7 = String(item_6)
 |23. Создать переменную item_7_type|let item_7_type;
 |24. Присвоить переменной item_7_type тип переменной item_7|item_7_type = typeof item_7;
 |25. Вывести в консоль тип данных item_7 в виде ——  “item_7 == ”  item_7,  “item_7_type == ”  item_7_type —— | console.log("item_7 == ", item_7,  "item_7_type == ", item_7_type)
 |26. Создать переменную “age_1” и присвоить ей значение 10|let age_1 = 10;
 |27. Создать переменную “age_2” и присвоить ей значение 18|let age_2 = 18;
 |28. Создать переменную “age_3” и присвоить ей значение 60|let age_3 = 60;
 |29. Создать if в котором будите проверять значение переменной age_1| - let compare_1 = <br>if (compare_1<br>  console.log()
 |30. Если age_1 < age_2, вывести в консоль “You don’t have access cause your age is ” + age_1 + “ It’s less then ”|let age_1 = 10; <br>let age_2 = 18; <br>let age_3 = 60;<br> let compare_1 = age_1 < age_2;<br> if (compare_1) <br>{console.log ("You don’t have access cause your age is " + age_1 + " It less then")};
 |31. Если age_1 >=  age_2 и age_1 <  age_3, вывести в консоль “Welcome  !”|let age_1 = 10;<br>let age_2 = 18;<br>let age_3 = 60;<br>let compare_1 = (age_1 >= age_2) && (age_1 < age_3)<br>if (compare_1) {<br>console.log("Welcome !")<br>}
 |32. Если age_1  > age_3, вывести в консоль “Keep calm and look Culture channel”.|let age_1 = 10;<br>let age_2 = 18;<br>let age_3 = 60;<br>let compare_1 = (age_1 > age_3)<br>if (compare_1) {<br>console.log("Keep calm and look Culture channel")<br>}
 |33. Иначе выводите “Technical work”.|let age_1 = 10;<br>let age_2 = 18;<br>let age_3 = 60;<br>let compare_1 = (age_1 > age_3)<br>if (compare_1) {  <br>console.log("Keep calm and look Culture channel")<br>}<br>else {<br>    console.log("Technical work")
 
 # Задания с разным количеством звездочек:)
# 1*
__Преобразовать написанный код в 26-33 пунктах в функцию, принимающую на вход возраст.__

		const checkAge = function(age) {if (age < age_2)
    	console.log("You don’t have access cause your age is", age, "It’s less then")
 		else if ((age >= age_2) && (age < age_3))
   		console.log("Welcome  !")
		else if (age > age_3)
   		 console.log("Keep calm and look Culture channel")
    	else
		console.log("Technical work")

		}
		checkAge(17)
__Вывести в консоль результат работы функции с возрастами "17"__

	[Running] node "c:\Users\Andrey\HW_1.js"
	You don’t have access cause your age is 17 It’s less then


	[Done] exited with code=0 in 0.048 seconds
__Вывести в консоль результат работы функции с возрастами "18"__

	[Running] node "c:\Users\Andrey\HW_1.js"
	Welcome  !


	[Done] exited with code=0 in 0.064 seconds
 
 __Вывести в консоль результат работы функции с возрастами "18"__

	[Running] node "c:\Users\Andrey\HW_1.js"
	Keep calm and look Culture channel


	[Done] exited with code=0 in 0.048 seconds
    
 # 2**
 __Преобразовать задание 1* таким образом, чтобы первым делом в функции проверялся тип данных. И если он не Number - кидалась ошибка.__
 
	let age_2 = 18;
	let age_3 = 60;


	const checkAge = function(age)
	{if (typeof age === 'number')
        	{if (age < age_2)
        	console.log("You don’t have access cause your age is", age, "It’s less then")
        	else if ((age >= age_2) && (age < age_3))
        	console.log("Welcome  !")
        	else if (age > age_3)
        	console.log("Keep calm and look Culture channel")
        	else
        	console.log("Technical work")}
	else
	console.log("Tha Data doesn't number")}

	checkAge(16)
    
   # 3***
   __Преобразовать 2* таким образом, чтобы значение '2' (строка в которой лежит ТОЛЬКО ЦИФРА) пропускалось, преобразовываясь в number__
   
	let age_2 = 18;
	let age_3 = 60;


	const checkAge = function(age){
	if (typeof age === 'string' && /^\d+$/.test(age))
   		age = Number(age)
	if (typeof age === 'number')
        {if (age < age_2)
        console.log("You don’t have access cause your age is", age, "It’s less then")
        else if ((age >= age_2) && (age < age_3))
        console.log("Welcome  !")
        else if (age > age_3)
        console.log("Keep calm and look Culture channel")
        else
        console.log("Technical work")
   	 }
	else
	console.log("Tha Data doesn't number")}
    checkAge("61")
    
 # 4****
__Преобразовать задание 3* таким образом, чтобы возраст вводится используя функцию prompt в привязанной верстке__

	let age_2 = 18;
	let age_3 = 60;

	const checkAge = function(age){
	if (typeof age === 'string' && /^\d+$/.test(age)){
   		let age = prompt("Enter your age");
    	age = Number(age)}
	if (typeof age === 'number')
        {if (age < age_2) 
        console.log("You don’t have access cause your age is", age, "It’s less then")
        else if ((age >= age_2) && (age < age_3))
        console.log("Welcome  !")
        else if (age > age_3)
        console.log("Keep calm and look Culture channel")
        else 
        console.log("Technical work")
    }
	else
	console.log("Tha Data doesn't number")}


	let userAge = prompt("Please enter your age: ")
	checkAge(userAge)
