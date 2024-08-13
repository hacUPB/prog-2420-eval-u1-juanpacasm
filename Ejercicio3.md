# Problema 1: Determinar el promedio de calificaciones de un estudiante y si ha aprobado o no
## Descripción del problema: Ana quiere saber si ha aprobado sus exámenes finales. Tiene una lista de sus calificaciones y necesita calcular el promedio. Para aprobar, debe tener un promedio de al menos 3.0.
```
inicio
    imprimir "señor usuario digite el numero de materias"
    leer n_mate
    notas=0
    R=0
    promed= notas/n_mate
    repetir
        imprimir "señor usuario digite la nota"
        leer not
        notas= notas + not
        R=R+1
    hata que n_mate=R
    si promed>3
        imprimir "felicidades señor usuario usted ha aprobado sus examenes, su promedio es de:"promed
    sino
        imprimir "señor usuario usted no aprobo sus examenes, su promedio es:"promed
fin
```

# Problema 4: Determinar la distancia total recorrida por un vehículo con registros de velocidad y tiempo
## Descripción del problema: María tiene un registro de las velocidades a las que ha conducido su vehículo y el tiempo que ha mantenido cada velocidad. Quiere calcular la distancia total recorrida.
```
inicio
    Definir ls_Vel
    Definir ls_tiem

    Leer ls_vel
    Leer ls_tiem

    Definir distancia_total = 0

    Para 1 desde 0 hasta longitud(ls_vel) - 1
        hacer vel_actual = ls_vel
        tiem_actual = ls_tiem
        
        Multiplicar vel_actiual por tiem_actual para obtener distancia
        
        sumar distancia_total a distancia e igualar a distancia_total

    Imprimir distancia_total
fin
```

# Problema 6(obligatorio): Calcular la edad de una persona a partir de su fecha de nacimiento y la fecha actual
## Descripción del problema: Se desea saber cuántos años, meses y días tiene actualmente una persona, basándose en su fecha de nacimiento. Además, le gustaría saber si ya ha cumplido años este año o aún no, y si hoy es su cumpleaños para celebrarlo. Cada una de las fechas está conformada por 3 variables: día, mes y año.
```
inicio
    leer dia_actual
    leer mes_actual
    leer año_actual
    imprimir "señor usuario digite su año de nacimiento"
    leer año
    imprimir "señor usuario digite su mes de nacimiento"
    leer mes
    imprimir "señor usuario digite su día de nacimiento"
    leer dia
    A=año_actual-año
    B=mes_actual-mes
    C=dia_actual-dia
    D= A-1
    si A=0 entonces
        si B=0 entonces
            si C=0 entonces
                imprimir "Usted nació hoy por lo tanto su edad es 0 años con 0 meses y 0 días"
            sino entonces
                imprimir "Su edad es 0 años con 0 meses y {C} días" 
            fin si
        sino entonces
            imprimir "Su edad es 0 años con {B} mese y {C} días"
        fin si
    sino entonces
        si B=0 entones
            si C=0 entonces
                imprimir "Feliz cumpleaños :D su edad es {A} años"
            sino entonces
                si C>0 entonces
                    imprimir "Usted ya cumplio años su edad es {A} años {B} meses {C} días"
                sino entonces
                    imprimir "Tú cumpleaños no ha pasado, tu edad es {D} años {B} meses {C} días"
                fin si
            fin si
        sino entonces
            si B>0 entonces
                imprimir "Usted ya cumplio años su edad es {A} años {B} meses {C} días"
            sino entonces
                imprimir "Tú cumpleaños no ha pasado tu edad es {D} años {B} meses {C} días"
            fin si
        fin si
    fin si


    

fin
```

-------------------------
ejemplo en clase parqueadero
```
inicio
    Costo=0
    imprimir "señor usuario digite la cantidad de horas"
    leer H
    si H<=2 entonces
        Costo=H*5
    sino 
        si H<=5 entonces
            Costo=10+(H-2)*4
        sino 
            si H<=10 entonces
                Costo=22+(H-5)*3
            sino 
                Costo=H*2
            fin si
        fin si
    fin si
    imprimir "señor usuario el costo del parqueadero es:" Costo

    
   
fin
```