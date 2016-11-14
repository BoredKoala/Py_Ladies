# Py_Ladies
#Repozytorium z nauki Pythona w trakcie warsztatów Py Ladies

czy_kontynuowac = "T"
while czy_kontynuowac == "T":
	plec = input("Podaj swoja plec (K/M)")
	waga = float(input("Podaj swoja wage w kg"))
	wzrost = float(input("Podaj swoj wzrost w metrach"))
	
	BMI = waga/(wzrost**2)
	print(BMI)
	if plec == "K":
		if BMI<16.5:
			print("Anoreksja")
		elif 16.5<BMI<20:
			print ("Niedowaga")
		elif 20<BMI<25:
			print ("Norma")
		elif 25<BMI<30:
			print ("Nadwaga")
		elif BMI>30:
			print ("Otyłość")
	elif plec == "M":
		if BMI<18.5:
			print("Anoreksja")
		elif 18.5<BMI<22.5:
			print ("Niedowaga")
		elif 22.5<BMI<27.5:
			print ("Norma")
		elif 27.5<BMI<32.5:
			print ("Nadwaga")
		elif BMI>32.5:
			print ("Otyłość")
	czy_kontynuowac = input("czy chcesz wyliczyc BMI jeszcze raz?T/N")
