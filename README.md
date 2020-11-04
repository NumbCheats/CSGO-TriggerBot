# CSGO-TriggerBot
A C++ External TriggerBot

The Trigger bot will automaticly shoot when your crosshair is on an enemy. 

IF you would like to add so when a key is held down, it will activate it, you need to replace this:

        mouse_event(MOUSEEVENTF_LEFTDOWN, NULL, NULL, 0, 0);
	mouse_event(MOUSEEVENTF_LEFTUP, NULL, NULL, 0, 0);
	Sleep(100);
				
	TO this:
				
				
				
   if (getAsyncKeyState(VK_RBUTTON) //Right Mouse Button
    {
    mouse_event(MOUSEEVENTF_LEFTDOWN, NULL, NULL, 0, 0);
    mouse_event(MOUSEEVENTF_LEFTUP, NULL, NULL, 0, 0);
    Sleep(100); //Optional
    }
       

You will need to update offsets sometimes, i have another repository on my github with all offsets
