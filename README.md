# Get_Cheapest_Agile_Period
Find the cheapest contiguous period on an Agile tariff to deliver a certain amount of charge

Designed to run on an ESP32.
In the code, change the following lines:

  //How much charge in kWh do you want to put into the battery tonight?
  const float ChargekWh = 10; 
  
  //What battery charge power have you set on the Inverter?
  const float ChargePower = 2.5; 

In the above, I want to put 10kWh into my batteries and I want them to charge at 2.5kW.

I have a Solis Inverter & find if I charge above 2.5kW, the cooling fans switch on & wake everyone up!
However with the 12kWh of batteries I have, that's plenty!

This is the next bit of the puzzle in automating the battery charging from the mains.  Now need to incorporate 
the current battery state of charge and the solar forcast to decide how much, if at all, to charge the battery - 
and send that setting to the Inverter.
