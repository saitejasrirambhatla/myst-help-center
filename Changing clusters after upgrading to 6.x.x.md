

### <u>**changing the targets of the blueprint after upgrading to 6.x.x**</u> 

**Pre upgrade:**

Go to the model and select  Actions => Control and  run custom action ‘properties’ as shown below

![](C:\Users\admin\Desktop\1283\custom.png)





 - Now copy the properties from the output of execution log and save it any where.

![](C:\Users\admin\Desktop\1283\execution log.png)

<u>Note:</u> You have to capture the properties of every blue print and save the output of each model seperately  any where in seperate files (should only need one model per blueprint).

**Upgrade to the latest version:**

- Login to MyST studio host and navigate to **MyST Home /bin** directory.
- Now upgrade to the latest version using upgrade.sh script by **./upgrade.sh 6.x.x**

**Post upgrade:**

- After upgrading again go to the model > actions and run the custom 'properties' action.

![](C:\Users\admin\Desktop\1283\custom.png) 



- Now copy the properties from the output of execution log and save it any where.

![](C:\Users\admin\Desktop\1283\execution log.png)

<u>Note:</u> You have to capture the properties of every blue print and save the output of each model seperately  any where in seperate files (should only need one model per blueprint).



**Compare the properties :**

- Now compare the properties of each model from 5.x.x version with  6.x.x version.
- For instance take the example of below properties of 5.x.x version.

![](C:\Users\admin\Desktop\1283\5.9.1.png)

As you see in the above image  the target  of **JdbcDataSource-107** is **osb cluster**.

- Now after upgrade compare the value in 6.x.x version.

![](C:\Users\admin\Desktop\1283\6.3.1.png)





As you see in the above image the target has changed to **soa_cluster**.



- In the same way compare the properties of each blueprint of the 5.x.x version with 6.x.x version

<u>Note:</u> If you do not notice any changes it is fine.

**Change the clusters :**

Now change the clusters which are changing in 6.x.x version to the previous values in the blueprint.


