gem "matrix"
require "matrix"
a = Array.new #строка 
m = 0 #счетчик кол-ва чисел в строке
b = []  #массив для преобразования текущей строки a в целочисленный массив
c = Array.new (m) #конечная двумерная матрица 
v = [] #значение предыдущей строки 
loop do  
	m=0
	a = gets.chomp
	puts "Текущий a: #{a}"
	if a == "" && v == ""
		break
	end
	v = a
	puts "Текущий v: #{v}"
	if a != ""
	    m ++
        m += a.count(",") 
        b = a.split(',')
	    for i in 0..m
	        b[i] = b[i].to_i
        end
        c += [b] 
	end
end
puts "#{c}"
puts "#{Matrix[*c].square?}"
if Matrix[*c].square? == true
       puts "#{Matrix[*c].det}"
end
STDIN.getc
