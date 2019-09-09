//Unit Conversion Program

// using C++14 GCC Compiler..................................

#include <iostream>
#include <string>

using namespace std;

void currency_Conversion(){
    cout<<"\n-----------CURRENCY CONVERSION ---------\n";
    
     int ini_currency,sec_currency ,first_amount;
    string Curr[4]{"Rupee","Dollar","Euro","Japanese Yen"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<<Curr[i]<<endl;
        }
    cout<<"\nWhich currency you Have (Please Input from given list) : ";
    cin>>ini_currency;
    cout<<"Enter "<<Curr[ini_currency-1]<<" Amount : ";
    cin>>first_amount;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_currency-1))
            Curr[i]=Curr[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<<Curr[i]<<endl;
        }
     cout<<"\nConvert into  (Please Input from given list) : ";
     cin>>sec_currency;
     
     
     if(ini_currency==1){
                if(sec_currency==1){
                    cout<<"Doller : "<<first_amount*0.014<<endl;
                }else if(sec_currency==2){
                     cout<<"Euro : "<<first_amount*0.013<<endl;
                }else if(sec_currency==3){
                     cout<<"Japanese Yen : "<<first_amount*1.49<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_currency==2){
             if(sec_currency==1){
                    cout<<"Rupee : "<<first_amount*71.74<<endl;
                }else if(sec_currency==2){
                     cout<<"Euro : "<<first_amount*0.91<<endl;
                }else if(sec_currency==3){
                     cout<<"Japanese Yen : "<<first_amount*106.30<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl<<endl; 
                    }
        }else if(ini_currency==3){
              if(sec_currency==1){
                    cout<<"Rupee : "<<first_amount*78.9<<endl;
                }else if(sec_currency==2){
                     cout<<"Doller: "<<first_amount*1.10<<endl;
                }else if(sec_currency==3){
                     cout<<"Japanese Yen : "<<first_amount*117.04<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_currency==4){
              if(sec_currency==1){
                    cout<<"Rupee : "<<first_amount*0.67<<endl;
                }else if(sec_currency==2){
                     cout<<"Doller: "<<first_amount*0.0094<<endl;
                }else if(sec_currency==3){
                     cout<<"Euro : "<<first_amount*0.0085<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
    }
    
    
void weight_Conversion(){
    cout<<"\n-----------WEIGHT CONVERSION ---------\n";
    
     int ini_weight,sec_weight,first_weight;
    string weight[4]{"kg","g","mg","pound"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<<weight[i]<<endl;
        }
    cout<<"\nWhich weight you Have (Please Input from given list) : ";
    cin>>ini_weight;
    cout<<"Enter "<<weight[ini_weight-1]<<" Amount : ";
    cin>>first_weight;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_weight-1))
           weight[i]=weight[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<<weight[i]<<endl;
        }
     cout<<"\nConvert into (Please Input from given list) : ";
     cin>>sec_weight;
     
     
     if(ini_weight==1){
                if(sec_weight==1){
                    cout<<"kg to g: "<<first_weight*1000<<endl;
                }else if(sec_weight==2){
                     cout<<"kg to mg : "<<first_weight*1000000<<endl;
                }else if(sec_weight==3){
                     cout<<"kg to pound: "<<first_weight*2.205<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_weight==2){
             if(sec_weight==1){
                    cout<<"g to kg : "<<first_weight*0.001<<endl;
                }else if(sec_weight==2){
                     cout<<"g to mg : "<<first_weight*1000<<endl;
                }else if(sec_weight==3){
                     cout<<"g to pound : "<<first_weight*0.0022<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl<<endl; 
                    }
        }else if(ini_weight==3){
              if(sec_weight==1){
                    cout<<"mg to kg : "<<first_weight*0.000001<<endl;
                }else if(sec_weight==2){
                     cout<<"mg to g : "<<first_weight*0.001<<endl;
                }else if(sec_weight==3){
                     cout<<"mg to pound : "<<first_weight*2.205*0.000001<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_weight==4){
              if(sec_weight==1){
                    cout<<"pound to kg : "<<first_weight*0.454<<endl;
                }else if(sec_weight==2){
                     cout<<"pound to g : "<<first_weight*453.592<<endl;
                }else if(sec_weight==3){
                     cout<<"pound to mg : "<<first_weight*453592.37<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
     
    }
    
void  length_Conversion(){
    cout<<"\n-----------LENGTH CONVERSION ---------\n";
    
     int ini_length,sec_length ,first_length;
    string length_unit[4]{"km","m","cm","mm"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<< length_unit[i]<<endl;
        }
    cout<<"\nWhich length you Have (Please Input from given list) : ";
    cin>>ini_length;
    cout<<"Enter "<< length_unit[ini_length-1]<<" length : ";
    cin>>first_length;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_length-1))
             length_unit[i]= length_unit[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<< length_unit[i]<<endl;
        }
     cout<<"\nConvert into (Please Input from given list) : ";
     cin>>sec_length;
     
     
     if(ini_length==1){
                if(sec_length==1){
                    cout<<"km to  m :"<<first_length*1000.0<<endl;
                }else if(sec_length==2){
                     cout<<"km to  cm :"<<first_length*100000.0<<endl;
                }else if(sec_length==3){
                     cout<<"km to  mm :"<<first_length*1000000.0<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_length==2){
             if(sec_length==1){
                    cout<<"m to km : "<<first_length*0.001<<endl;
                }else if(sec_length==2){
                     cout<<"m to cm : "<<first_length*100.0<<endl;
                }else if(sec_length==3){
                     cout<<"m to mm : "<<first_length*1000.0<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl<<endl; 
                    }
        }else if(ini_length==3){
              if(sec_length==1){
                    cout<<"cm to km : "<<first_length*0.00001<<endl;
                }else if(sec_length==2){
                     cout<<"cm to m : "<<first_length*0.01<<endl;
                }else if(sec_length==3){
                     cout<<"cm to mm : "<<first_length*10.0<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_length==4){
              if(sec_length==1){
                    cout<<"mm to km : "<<first_length*0.000001<<endl;
                }else if(sec_length==2){
                     cout<<"mm to m : "<<first_length*0.001<<endl;
                }else if(sec_length==3){
                     cout<<"mm to cm : "<<first_length*0.1<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
    }
void area_Conversion(){
    cout<<"\n-----------AREA CONVERSION ---------\n";
    
     int ini_area,sec_area ,first_area;
    string area_unit[4]{"km square","metre square","mile square","foot square"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<< area_unit[i]<<endl;
        }
    cout<<"\nWhich area you Have (Please Input from given list) : ";
    cin>>ini_area;
    cout<<"Enter "<< area_unit[ini_area-1]<<" area : ";
    cin>>first_area;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_area-1))
             area_unit[i]= area_unit[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<< area_unit[i]<<endl;
        }
     cout<<"\nConvert into  (Please Input from given list) : ";
     cin>>sec_area;
     
     
     if(ini_area==1){
                if(sec_area==1){
                    cout<<"km square to metre square :"<<first_area*1000000.0<<endl;
                }else if(sec_area==2){
                     cout<<"km square to mile square :"<<first_area*0.386<<endl;
                }else if(sec_area==3){
                     cout<<"km square to foot square :"<<first_area*10763910.4<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_area==2){
             if(sec_area==1){
                    cout<<"metre square  to km square: "<<first_area*0.000001<<endl;
                }else if(sec_area==2){
                     cout<<"metre square to mile square : "<<first_area*3.861*0.0000001<<endl;
                }else if(sec_area==3){
                     cout<<"metre square to foot square : "<<first_area*10.764<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }else if(ini_area==3){
              if(sec_area==1){
                    cout<<"mile square to km square : "<<first_area*2.59<<endl;
                }else if(sec_area==2){
                     cout<<"mile square to  metre square : "<<first_area*2589988.11<<endl;
                }else if(sec_area==3){
                     cout<<"mile square to foot square : "<<first_area*27878400<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_area==4){
              if(sec_area==1){
                    cout<<"foot square to km square : "<<first_area*9.29*0.00000001<<endl;
                }else if(sec_area==2){
                     cout<<"foot square to metre square : "<<first_area*0.0929<<endl;
                }else if(sec_area==3){
                     cout<<"foot square  to mile square : "<<first_area*3.587*0.00000001<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
    }
void fuel_Conversion(){
       cout<<"\n-----------PRESSURE CONVERSION ---------\n";
    
     int ini_fuel,sec_fuel ,first_fuel;
    string fuel_unit[4]{"Kilometre per litre","Miles per gallon (Imperial)","US Miles per gallon","Litre per 100 kilometres"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<< fuel_unit[i]<<endl;
        }
    cout<<"\nWhich fuel unit you Have (Please Input from given list) : ";
    cin>>ini_fuel;
    cout<<"Enter "<< fuel_unit[ini_fuel-1]<<" fuel : ";
    cin>>first_fuel;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_fuel-1))
             fuel_unit[i]= fuel_unit[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<< fuel_unit[i]<<endl;
        }
     cout<<"\nConvert into (Please Input from given list) : ";
     cin>>sec_fuel;
     
     
     if(ini_fuel==1){
                if(sec_fuel==1){
                    cout<<"Kilometre per litre to Miles per gallon (Imperial) :"<<first_fuel*2.825<<endl;
                }else if(sec_fuel==2){
                     cout<<"Kilometre per litre to US Miles per gallon :"<<first_fuel*2.352<<endl;
                }else if(sec_fuel==3){
                     cout<<"Kilometre per litre to Litre per 100 kilometres :"<<100.0/first_fuel<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_fuel==2){
             if(sec_fuel==1){
                    cout<<"Miles per gallon (Imperial)  to Kilometre per litre: "<<first_fuel/2.825<<endl;
                }else if(sec_fuel==2){
                     cout<<"Miles per gallon (Imperial) to US Miles per gallon : "<<first_fuel/1.201<<endl;
                }else if(sec_fuel==3){
                     cout<<"Miles per gallon (Imperial) to Litre per 100 kilometres : "<<282.481/first_fuel<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }else if(ini_fuel==3){
              if(sec_fuel==1){
                    cout<<"US Miles per gallon to Kilometre per litre : "<<first_fuel/2.352<<endl;
                }else if(sec_fuel==2){
                     cout<<"US Miles per gallon to  Miles per gallon (Imperial) : "<<first_fuel*1.201<<endl;
                }else if(sec_fuel==3){
                     cout<<"US Miles per gallon to Litre per 100 kilometres : "<<235.215/first_fuel<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_fuel==4){
              if(sec_fuel==1){
                    cout<<"Litre per 100 kilometres to Kilometre per litre : "<<100.0/first_fuel<<endl;
                }else if(sec_fuel==2){
                     cout<<"Litre per 100 kilometres to Miles per gallon (Imperial) : "<<282.481/first_fuel<<endl;
                }else if(sec_fuel==3){
                     cout<<"Litre per 100 kilometres  to US Miles per gallon : "<<235.215/first_fuel<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
    }
void time_Conversion(){
    cout<<"\n-----------TIME CONVERSION ---------\n";
    
     int ini_time,sec_time ,first_time;
    string time_unit[4]{"Second","Minute","Hour","Day"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<< time_unit[i]<<endl;
        }
    cout<<"\nWhich time unit you Have (Please Input from given list) : ";
    cin>>ini_time;
    cout<<"Enter "<< time_unit[ini_time-1]<<" time : ";
    cin>>first_time;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_time-1))
             time_unit[i]= time_unit[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<< time_unit[i]<<endl;
        }
     cout<<"\nConvert into (Please Input from given list) : ";
     cin>>sec_time;
     
     
     if(ini_time==1){
                if(sec_time==1){
                    cout<<"Second to Minute :"<<first_time/60.0<<endl;
                }else if(sec_time==2){
                     cout<<"Second to Hour :"<<first_time/3600.0<<endl;
                }else if(sec_time==3){
                     cout<<"Second to Day :"<<first_time/86400.0<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_time==2){
             if(sec_time==1){
                    cout<<"Minute  to Second: "<<first_time*60<<endl;
                }else if(sec_time==2){
                     cout<<"Minute to Hour : "<<first_time/60.0<<endl;
                }else if(sec_time==3){
                     cout<<"Minute to Day : "<<first_time/1440.0<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }else if(ini_time==3){
              if(sec_time==1){
                    cout<<"Hour to Second : "<<first_time*3600<<endl;
                }else if(sec_time==2){
                     cout<<"Hour to  Minute : "<<first_time*60<<endl;
                }else if(sec_time==3){
                     cout<<"Hour to Day : "<<first_time/24.0<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_time==4){
              if(sec_time==1){
                    cout<<"Day to Second : "<<first_time*86400<<endl;
                }else if(sec_time==2){
                     cout<<"Day to Minute : "<<first_time*1440<<endl;
                }else if(sec_time==3){
                     cout<<"Day  to Hour : "<<first_time*24<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
    }
void volume_Conversion(){
     cout<<"\n-----------VOLUME CONVERSION ---------\n";
    
     int ini_volume,sec_volume ,first_volume;
    string volume_unit[4]{"Litre","Mililitre","CubicMetre","CubicFoot"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<< volume_unit[i]<<endl;
        }
    cout<<"\nWhich volume unit you Have (Please Input from given list) : ";
    cin>>ini_volume;
    cout<<"Enter "<< volume_unit[ini_volume-1]<<" volume : ";
    cin>>first_volume;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_volume-1))
             volume_unit[i]= volume_unit[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<< volume_unit[i]<<endl;
        }
     cout<<"\nConvert into (Please Input from given list) : ";
     cin>>sec_volume;
     
     
     if(ini_volume==1){
                if(sec_volume==1){
                    cout<<"Litre to Mililitre :"<<first_volume*1000<<endl;
                }else if(sec_volume==2){
                     cout<<"Litre to CubicMetre :"<<first_volume/0.001<<endl;
                }else if(sec_volume==3){
                     cout<<"Litre to CubicFoot :"<<first_volume*0.0353147<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_volume==2){
             if(sec_volume==1){
                    cout<<"Mililitre  to Litre: "<<first_volume/1000.0<<endl;
                }else if(sec_volume==2){
                     cout<<"Mililitre to CubicMetre : "<<first_volume/1000000.0<<endl;
                }else if(sec_volume==3){
                     cout<<"Mililitre to CubicFoot : "<<(first_volume*3.531)/100000<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }else if(ini_volume==3){
              if(sec_volume==1){
                    cout<<"CubicMetre to Litre : "<<first_volume*1000.0<<endl;
                }else if(sec_volume==2){
                     cout<<"CubicMetre to  Mililitre : "<<first_volume*1000000.0<<endl;
                }else if(sec_volume==3){
                     cout<<"CubicMetre to CubicFoot : "<<first_volume*35.315<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_volume==4){
              if(sec_volume==1){
                    cout<<"CubicFoot to Litre : "<<first_volume*28.317<<endl;
                }else if(sec_volume==2){
                     cout<<"CubicFoot to Mililitre : "<<first_volume*28316.847<<endl;
                }else if(sec_volume==3){
                     cout<<"CubicFoot  to CubicMetre : "<<first_volume*0.0283<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
    }
void  temperature_Conversion(){
     cout<<"\n-----------TEMPREATURE CONVERSION ---------\n";
    
     int ini_temperature,sec_temperature ,first_temperature;
    string temperature_unit[3]{"Celsius","Fahrenheit","Kelvin"};
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<< temperature_unit[i]<<endl;
        }
    cout<<"\nWhich temperature unit you Have (Please Input from given list) : ";
    cin>>ini_temperature;
    cout<<"Enter "<< temperature_unit[ini_temperature-1]<<" temperature : ";
    cin>>first_temperature;
    for(int i{0};i<3;i++){
        if(i<2&&i>=(ini_temperature-1))
             temperature_unit[i]= temperature_unit[i+1];
    }
    for(int i{0};i<2;i++){
        cout<<i+1<<" : "<< temperature_unit[i]<<endl;
        }
     cout<<"\nConvert into (Please Input from given list) : ";
     cin>>sec_temperature;
     
     
     if(ini_temperature==1){
                if(sec_temperature==1){
                    cout<<"Celsius to Fahrenheit :"<<(first_temperature*(9/5.0))+32<<endl;
                }else if(sec_temperature==2){
                     cout<<"Celsius to Kelvin :"<<first_temperature + 273.15<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_temperature==2){
             if(sec_temperature==1){
                    cout<<"Fahrenheit  to Celsius: "<<(first_temperature-32)*(5.0/9)<<endl;
                }else if(sec_temperature==2){
                     cout<<"Fahrenheit to Kelvin : "<<(first_temperature-32)*(5.0/9)+273.15<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }else if(ini_temperature==3){
              if(sec_temperature==1){
                    cout<<"Kelvin to Celsius : "<<first_temperature-275.315<<endl;
                }else if(sec_temperature==2){
                     cout<<"Kelvin to  Fahrenheit : "<<(first_temperature-273.15)*(9/5.0)+32<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             }
        }
    
void  pressure_Conversion(){
        cout<<"\n-----------PRESSURE CONVERSION ---------\n";
    
     int ini_pressure,sec_pressure ,first_pressure;
    string pressure_unit[4]{"Atmospere","Bar","Pascal","Torr"};
    for(int i{0};i<4;i++){
        cout<<i+1<<" : "<< pressure_unit[i]<<endl;
        }
    cout<<"\nWhich pressure unit you Have (Please Input from given list) : ";
    cin>>ini_pressure;
    cout<<"Enter "<< pressure_unit[ini_pressure-1]<<" pressure : ";
    cin>>first_pressure;
    for(int i{0};i<4;i++){
        if(i<3&&i>=(ini_pressure-1))
             pressure_unit[i]= pressure_unit[i+1];
    }
    for(int i{0};i<3;i++){
        cout<<i+1<<" : "<< pressure_unit[i]<<endl;
        }
     cout<<"\nConvert into (Please Input from given list) : ";
     cin>>sec_pressure;
     
     
     if(ini_pressure==1){
                if(sec_pressure==1){
                    cout<<"Atmospere to Bar :"<<first_pressure*1.013<<endl;
                }else if(sec_pressure==2){
                     cout<<"Atmospere to Pascal :"<<first_pressure*101325.0<<endl;
                }else if(sec_pressure==3){
                     cout<<"Atmospere to Torr :"<<first_pressure*760.0<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
         }else if(ini_pressure==2){
             if(sec_pressure==1){
                    cout<<"Bar  to Atmospere: "<<first_pressure/1.013<<endl;
                }else if(sec_pressure==2){
                     cout<<"Bar to Pascal : "<<first_pressure/100000.0<<endl;
                }else if(sec_pressure==3){
                     cout<<"Bar to Torr : "<<first_pressure*750.062<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }else if(ini_pressure==3){
              if(sec_pressure==1){
                    cout<<"Pascal to Atmospere : "<<first_pressure/101325.0<<endl;
                }else if(sec_pressure==2){
                     cout<<"Pascal to  Bar : "<<first_pressure*100000.0<<endl;
                }else if(sec_pressure==3){
                     cout<<"Pascal to Torr : "<<first_pressure/133.322<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
             
        }else if(ini_pressure==4){
              if(sec_pressure==1){
                    cout<<"Torr to Atmospere : "<<first_pressure*28.317<<endl;
                }else if(sec_pressure==2){
                     cout<<"Torr to Bar : "<<first_pressure/760.0<<endl;
                }else if(sec_pressure==3){
                     cout<<"Torr  to Pascal : "<<first_pressure*133.322<<endl;
                }else{
                    cout<<" Wrong Input! Please select correct option. "<<endl; 
                    }
        }
    }
int main()
    {
    cout<<"------WELCOME TO UNIT CONVERSION APPLICATION-----\n\n";
    cout<<"1 . Currency "<<endl;
    cout<<"2 . Weight "<<endl;
    cout<<"3 . Length "<<endl;
    cout<<"4 . Area "<<endl;
    cout<<"5 . Fuel "<<endl;
    cout<<"6 . Time "<<endl;
    cout<<"7 . Volume "<<endl;
    cout<<"8 . Temperature "<<endl;
    cout<<"9 . Pressure "<<endl<<endl;
    cout<<"press 10 for Exit : "<<endl<<endl;
    cout<<"Choose option for Conversion : ";
    int select_option {0};
    do{
    cin>>select_option;
    if(!(select_option>=1&&select_option<=10)){
        cout<<" Wrong Input!!\nPlease select correct option.....\n";
        }
    }while(!(select_option>=1&&select_option<=10));
    
    switch(select_option)
    {
    case 1:
     currency_Conversion();
     break;
    
    case 2:
      weight_Conversion();
      break;
    
    case 3:
     length_Conversion();
     break;
    
    case 4:
      area_Conversion();
      break;
    
    case 5:
     fuel_Conversion();
     break;
    
    case 6:
      time_Conversion();
      break;
      
    case 7: 
      volume_Conversion();
      break;
      
    case 8:
      temperature_Conversion();
      break;

    case 9:
      pressure_Conversion();
      break;
    case 10:
      exit(0);
      default:{
          cout<<"/n Thank you ";
          }
    }
    return 0;
   }
