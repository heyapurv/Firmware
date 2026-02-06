## To change the logo 
![alt text](image.png)


1. Go to : ``` make menuconfig```
2. Select PAYLOAD 
    - select edk2 Bootsplash path and filename
    - change the path and file name with your custom logo 

    ![alt text](<image1.png>)

3. Add 24 Bit .BMP image file at this location : /coreboot/Documentation/ 

4. Save + OK + Exit 

5. make the build again 
   run : ```make```

6. Test the build in qemu 

7. 
![alt text](image-1.png)

- successfully changed the logo 


## Customize the Setup Page 

![alt text](image-2.png)

- To make changes on this front page got to 
``` /coreboot/payloads/external/edk2/workspace/tianocore/MdeModulePkg/Application/UiApp ```

- Make the required changes in ``` FrontPageStrings.uin``` file 
- Also add the newly added strings to ``` FrontPageVfr.Vfr ``` file 

outcome : 

![alt text](image-3.png)