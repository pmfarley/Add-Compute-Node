# Add-Compute-Node

Adding a compute node to an OpenShift Cluster with Assisted Installer

Perform the following steps to add new hosts to an OpenShift cluster. 
This process will generate a new Discovery ISO that you will use to "Add hosts” to your OpenShift cluster from the Red Hat Hybrid Cloud Console on https://console.redhat.com/openshift.

## **Step 1.  Open the Red Hat Hybrid Cloud Console**

Open the Assisted Installer page:  https://console.redhat.com/openshift.

## **Step 2. Select Cluster**

Find and select your cluster from the list, use the filter if necessary:

![image](https://user-images.githubusercontent.com/48925593/167686892-c4fb7632-b4bf-4d9f-998f-b43fffed3cdd.png)


## **Step 3. Select ‘Add Hosts’**

Select ‘**Add Hosts**’ from the items selected.  

![image](https://user-images.githubusercontent.com/48925593/167687016-f35bed95-1389-4dff-8cae-795c646abd50.png)


 
## **Step 4. Select ‘Add Hosts’**
Select ‘**Add Hosts**’ to generate a new Discovery ISO. 

![image](https://user-images.githubusercontent.com/48925593/167687126-d980957d-c300-466e-92f2-e63250ef3606.png)



## **Step 5. Generate Discovery ISO**

Select ‘**Generate Discovery ISO**’; optionally change the selection for a Full image file, or a Minimal image file.

![image](https://user-images.githubusercontent.com/48925593/167687265-04422eb7-e811-4b64-8c85-31b454241038.png)


 
## **Step 6.  Download Discovery ISO**

To download the new Discovery ISO file, select ‘Download Discovery ISO’.  
When complete, select ‘**Close**’.  

![image](https://user-images.githubusercontent.com/48925593/167687299-528a20a2-a377-454d-a562-7a250dee82b9.png)



## **Step 7.  Boot Host to Discovery ISO & Install**

Boot new host server(s) from the new Discovery ISO, then continue with the process when they’ve been discovered by selecting ‘**Install ready hosts**’.  
Follow the installation progress, by optionally selecting ‘**View cluster events**’.

![image](https://user-images.githubusercontent.com/48925593/167687357-56f11ff6-d802-4eef-a79d-bd48c41ad926.png)



## **Step 8. Complete Installation**

When complete, the installer will show a status of ‘**installed**’.  
The Cluster Events will show a message: 
“Please check console for progress and to possibly approve pending CSRs)”


## **Step 9. Approve CSRs**

Login to the OpenShift console and navigate to Compute > Nodes and select the new host, and select ‘**Approve**’.
You can also use the oc command line utility to approve the pending CSR request.

![image](https://user-images.githubusercontent.com/48925593/167687444-c7a35e72-f2c9-4e76-978c-92bfbe23a0b1.png)



## **Step 10. Approve any additional CSR’s**

![image](https://user-images.githubusercontent.com/48925593/167687483-928a4a4e-34c0-4d63-be7d-24054e7dd460.png)


## **Step 11. Complete. Node Ready**

When this process is complete, the new host should be in a ‘**Ready**’ state.  

![image](https://user-images.githubusercontent.com/48925593/167687530-fec75e21-ed64-4575-b066-6ecb61487f16.png)


