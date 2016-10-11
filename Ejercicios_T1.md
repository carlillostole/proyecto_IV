**Ejercicios tema 1: Introducción a la infraestructura virtual: concepto y soporte físico**

#**EJERCICIO 1**
**Consultar en el catálogo de alguna tienda de informática el precio de un ordenador tipo servidor y calcular su coste de amortización a cuatro y siete años**

En mi caso voy a realizar los cálculos sobre el pc ![http://store.hp.com/SpainStore/Merch/Product.aspx?id=P1J95EA&opt=ABE&sel=DTP](PC All In One HP Envy 27-p001ns).


Suponemos que el ordenador se compra a principios de año, tenemos que quitarle el IVA, que es el 21% del precio que pagamos del artículo. Dicho pc tiene un precio de 1999,00€, sin le quitamos el IVA se queda en 1652,06€.

**Amortización a los 4 años**: Si consideramos que cada año tiene una amortización máxima de un 25%, el servidor nos costaria 1652,06 * 0.25 = 413.01 € cada año.
**Amortización a los 7 años**: Si consideramos que se amortiza más los primeros años y menos los últimos años, por cada año tendriamos:
Primer año : 1652,06 * 0.25 = 413.01€
Segundo año : 1652,06 * 0.25 = 413.01€
Tercer y cuarto año : 1652,06 * 0.15 = 247.80€
Quinto año : 1652,06 * 0.10 = 165.20€
Sexto y séptimo año : 1652,06 * 0.05 = 82.60€
s

#**EJERCICIO 2**
**Usando las tablas de precios de servicios de alojamiento en Internet y de proveedores de servicios en la nube, Comparar el coste durante un año de un ordenador con un procesador estándar (escogerlo de forma que sea el mismo tipo de procesador en los dos vendedores) y con el resto de las características similares (tamaño de disco duro equivalente a transferencia de disco duro) en el caso de que la infraestructura comprada se usa sólo el 1% o el 10% del tiempo**

**Servidor dedicado:** AMD Opteron™ 4274 HE, 8 Cores x 2.6 GHz(3.5 GHz Turbo Core), 16 GB DDR3 ECC, 1,500 GB (2 x 1,500 GB SATA).
**Servidor cloud:**Servidor Cloud FLEX, vCores: 8 x 2,0 GHz, 16 GB RAM, 500 GB SSD.

Uso de 1%:

-Servidor dedicado: 119,99 euros/mes * 12 meses = 1439,88 euros/año.
-Servidor cloud: 208,80 €/mes * 12 meses * 0.01 = 25,05 euros/mes.

Uso de 10%:

-Servidor dedicado: 119,99 euros/mes * 12 meses = 1439,88 euros/año.
-Servidor cloud: 208,80 €/mes * 12 meses * 0.10 = 250,5 euros/mes.

#**EJERCICIO 3**
**Qué tipo de virtualización usarías en cada caso? Comentar en el foro.**
**Crear un programa simple en cualquier lenguaje interpretado para Linux, empaquetarlo con CDE y probarlo en diferentes distribuciones**

Al ser un programa simple he creado el Hola Mundo!!.

Instalo el programa CDE mediante el comando: sudo apt-get install cde

A continuación ejecuto el programa PRUEBA.py: cde python PRUEBA.py


![](fotooooo py).


#**EJERCICIO 4**
**Comprobar si el procesador o procesadores instalados tienen estos flags. ¿Qué modelo de procesador es? ¿Qué aparece como salida de esa orden?**

Mediante el comando **egrep '^flags.*(vmx|svm)' /proc/cpuinfo** comprobamos que el flag vmx está activado:

root@carlillostole:/home/carlillostole# egrep '^flags.*(vmx|svm)' /proc/cpuinfo

flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf eagerfpu pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm epb tpr_shadow vnmi flexpriority ept vpid fsgsbase smep erms xsaveopt dtherm ida arat pln pts

Flag vmx activado, por tanto es posible la virtualización.

Con el comando **cat /proc/cpuinfo** vemos el modelo de procesador de mi pc:

Intel(R) Core(TM) i7-3630QM CPU @ 2.40GHz


#**EJERCICIO 5**
**1.Comprobar si el núcleo instalado en tu ordenador contiene este módulo del kernel usando la orden kvm-ok.**
**2.Instalar un hipervisor para gestionar máquinas virtuales, que más adelante se podrá usar en pruebas y ejercicios.**

**1**
Primero instalamos el paquete cpu-checker: sudo apt-get install cpu-checker
Introducimos el comando kvm-ok y la respuesta es:

root@carlillostole:/home/carlillostole# kvm-ok
INFO: /dev/kvm exists
KVM acceleration can be used
root@carlillostole:/home/carlillostole# 

Por tanto puedo usar la aceleración por hardware del procesador.

**2**

Tengo instalado virtualbox y vagrant.


















   




