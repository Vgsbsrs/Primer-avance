/******************************************************************************
                           Primer avance
Aziz Jorge Eduardo Alejo Reyes
*******************************************************************************/
#include <iostream>
using namespace std;

int main(){
    int salir, num, h, desi, preciotratamiento, cantidad, preciounitario, opc;
    int total=0;
    char des[3], nom[3];
    
    do{
cout<<"1.- Agendar cita"<<endl;
cout<<"2.- Modificar cita"<<endl;
cout<<"3.- Eliminar cita"<<endl;
cout<<"4.- Lista de citas vigentes"<<endl;
cout<<"5.- Limpiar pantalla"<<endl;
cout<<"6.- Salir"<<endl;
cout<<"Elija opción: "; cin>>opc;
cout<<"*****";

switch(opc){
    
case 1:

   do{
    cout<< "ingrese el numero de la cita: "<<endl;
       cin>>num;
    cout<< "ingrese su nombre: "<<endl;
       cin>>nom;  
    cout<< "ingrese la hora del tratamiento : "<<endl;
       cin>>h;
    cout<< "mencione una breve descripcion del tratamiento : "<<endl;
       cin>>des;
    cout<<"Cuanto cuesta el tratamiento"<<endl;
      cin>>preciotratamiento;
    cout<<"escriba la cantidad del tratamiento"<<endl;
      cin>>cantidad;
    cout<<"ingrese el precio unitario"<<endl;
    cin>>preciounitario;
    total=(preciotratamiento*cantidad)+preciounitario;
    cout<<"El total a pagar es: "<<total<<endl;
    cout<<"Tarea realizada con exito"<<endl;
    cout<<"desea agendar una cita? Ingrese 1 si desea continuar 2 si desea cancelar"<<endl;
      cin>>desi;  
  }
  while(desi==1);
     break;
     
case 2:
     break;
     
case 3:
     break;
     
case 4:
     break;
     
case 5:
     break;
     
case 6:
    exit(1);
     break;
     
default:
    cout<<"Opcion incorrecta, ingrese alguna de las opciones disponibles"<<endl;
}

cout<<"Para volver al menu ingrese 1 para salir 2"<<endl;
cin>>salir;
}
    while(salir==1);
    return 0;
}
