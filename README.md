# avrdude-syti
avrdude setup for microchip studio

1. Clone Github Repository to a location which preferably isn't your Downloads folder

2. Open ```Microchip Studio```

3. Open ```Tools``` in menu bar

4. Open ```External Tools``` in the dropdown

4. ```Title```: ```Send to arduino```

5. ```Command```: ```PATH_TO_AVRDUDE.exe```

6. ```Arguments```: ```-C "PATH_TO_AVRDUDE.conf" -p atmega328p -c arduino -P COM3 -b 115200 -U flash:w:"$(ProjectDir)Debug/$(TargetName).hex":i```
