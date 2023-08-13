# DATA-ACQUISITION-SYSTEM-TO-INTERFACE-ADC-WITH-8051
Main objective is to build an 8051 based data acquisition system to interface analog to digital converter (ADC 0808) to read potentiometer based voltage divider and display the value on LCD display

# Analog-to-digital-converter
Build an 8051 based data acquisition system to interface analog to digital converter to read potentiometer based voltage divider and display the value on LCD display

# Interfacing ADC0808 with 8051 Microcontroller
ADC is the Analog to Digital converter, which converts analog data into digital format; usually it is used to convert analog voltage into digital format. Analog signal has infinite no of values like a sine wave or our speech, ADC converts them into particular levels or states, which can be measured in numbers as a physical quantity. Instead of continuous conversion, ADC converts data periodically, which is usually known as sampling rate. Telephone modem is one of the examples of ADC, which is used for internet, it converts analog data into digital data, so that computer can understand, because computer can only understand Digital data. The major advantage, of using ADC is that, we noise can be efficiently eliminated from the original signal and digital signal can travel more efficiently than analog one. That’s the reason that digital audio is very clear, while listening.

# ADC0808
ADC0808/0809 is a monolithic CMOS device and microprocessor compatible control logic and has 28 pin which gives 8-bit value in output and 8- channel ADC input pins (IN0-IN7). Its resolution is 8 so it can encode the analog data into one of the 256 levels (28). This device has three channel address line namely: ADDA, ADDB and ADDC for selecting channel. Below is the Pin Diagram for ADC0808

![image](https://github.com/tejas6129/DATA-ACQUISITION-SYSTEM-TO-INTERFACE-ADC-WITH-8051/assets/127325785/731cc629-67ff-49a7-b365-813746413285)


ADC0808 requires a clock pulse for conversion. We can provide it by using oscillator or by using microcontroller. In this project we have applied frequency by using microcontroller.

# Circuit Diagram:
![image](https://github.com/tejas6129/DATA-ACQUISITION-SYSTEM-TO-INTERFACE-ADC-WITH-8051/assets/127325785/0c5ffa73-e0cf-41df-9616-b79f9c733ab7)


# Working:
In this project we have interfaced three channels of ADC0808. And for demonstration we have used three variable resistors. When we power the circuit then microcontroller initialize the LCD by using appropriate command, gives clock to ADC chip, selects ADC channel by using address line and send start conversion signal to ADC. After this ADC first reads selected ADC channel input and gives its converted output to microcontroller. Then microcontroller shows its value at Ch1 position in LCD. And then microcontroller changes ADC channel by using address line. And then ADC reads selected channel and send output to microcontroller. And show on LCD as name Ch2. And like wise for other channels.

![image](https://github.com/tejas6129/DATA-ACQUISITION-SYSTEM-TO-INTERFACE-ADC-WITH-8051/assets/127325785/55a924d9-2d9f-48b7-bc6f-995cc98e9808)



# Circuit Designing:
![image](https://github.com/tejas6129/DATA-ACQUISITION-SYSTEM-TO-INTERFACE-ADC-WITH-8051/assets/127325785/18aeee25-aa76-4212-b065-102cb176fdfc)


![image](https://github.com/tejas6129/DATA-ACQUISITION-SYSTEM-TO-INTERFACE-ADC-WITH-8051/assets/127325785/690d999d-4ef5-4ade-b04c-ad29cdba032e)


# ADC Display output:
![image](https://github.com/tejas6129/DATA-ACQUISITION-SYSTEM-TO-INTERFACE-ADC-WITH-8051/assets/127325785/199511e1-a8d3-45c7-a4d5-b5fd3029f6ad)

