# Proyecto-de-la-empresa-S.A
class vendedor:

    def __init__(self,):

        self.





    def crear_venta_pasaje(self,CVP):

#Agregar la venta y su detalle en las tablas correspondientes. 

#Considerar que la venta de un pasaje ocupa una vacante en un bus





    def emitir_pasaje(self, EP):

#El pasaje muestra los siguientes datos: folio, fecha, hora, nombre pasajero, origen-destino, hora de salida, patente del bus, chofer, auxiliar y precio 





    def reporte_listados_de_pasajeros_bus(self, RLDPB):        



#----------------------------------------------------------------------------------------



class chofer:

    def __initi__(self, id, nombre, contraseña, salario  ):#la contra que sea de text y minimo 4 y max 10

        if type(id) == int:

            self.__id = id

        else:

            raise ValueError("error tiene ques ser numero")

        self.nombre = nombre



        if type(contraseña) == str:

            self.__contraseña = contraseña

        else:

            raise ValueError("error tiene que ser texto")

        

        self.salario = salario









    @property

    def contraseña(self):

        return self.__contraseña    



    @contraseña.setter

    



    @property

    def id(self):

        return self.__id

    



    def marca_asistencia(self, MA):#si va a asistir en el bus



    def reporte_listados_de_pasajeros_bus(self, RLDPB):#lista de pasajeros





#----------------------------------------------------------------------------------------





class jefe_operacion:

    def __init__(self,):

        self.





    def planificacion_viajes(self,PV):

#Agregar, a la base de datos, nuevas salidas de buses con: destino, hora salida, chofer y auxiliar. 

#Controlar las horas de conducción de los choferes, dato a considerar en el punto anterior

        



    def reporte_venatas_realizadas(self, R):

#Mostrar en pantalla las ventas realizadas en una fecha específica (sólo tiene acceso el jefe de operaciones





    def reporte_listados_de_pasajeros_bus(self, RLDPB):  





#----------------------------------------------------------------------------------------





class pasajero:

    def __init__ (self, ):















#----------------------------------------------------------------------------------------



class bus:

    def __init__(self, patente, destino, chofer_asignado,    ):

        self.



    def cantidad_pasajeros





import sqlite3



try:

    cnn = sqlite3.connect("cuenta_corriente.db")

    

    cnn.execute("create table if not exists vendedor()")

    

    cnn.execute("create table if not exists chofer ()")



    cnn.execute("create table if not exists jefe_operacion ()")



    cnn.execute("create table if not exists bus ()")





    cnn.execute("insert into  ()values()", ()) 

    



    cnn.commit()

    

except sqlite3.IntegrityError as ex:

    print("usuario existe", ex)

    

except sqlite3.OperationalError as ex:

    print("error en la query", ex)



except Exception as ex:

    print("error base de datos", type(ex))



finally:

    print("progranma terminado")

    
