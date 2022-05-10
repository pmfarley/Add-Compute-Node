# Add-Compute-Node

Adding a compute node to an OpenShift Cluster with Assisted Installer

Perform the following steps to add new hosts to an OpenShift cluster. 
This process will generate a new Discovery ISO that you will use to "Add hosts” to your OpenShift cluster from the Red Hat Hybrid Cloud Console on console.redhat.com/openshift.

## **Step 1.  Open the Red Hat Hybrid Cloud Console**

Open the Assisted Installer page:  console.redhat.com/openshift.

## **Step 2. Select Cluster**

Find and select your cluster from the list, use the filter if necessary:

![image](https://user-images.githubusercontent.com/48925593/167685522-81911e62-2d57-4335-a31b-3152e3f58df5.png)


## **Step 3. Select ‘Add Hosts’**

Select ‘**Add Hosts**’ from the items selected.  

![image](https://user-images.githubusercontent.com/48925593/167685689-10ba28f5-90fd-4136-967d-06ec61ef904b.png)

 
## **Step 4. Select ‘Add Hosts’**
Select ‘**Add Hosts**’ to generate a new Discovery ISO. 

![image](https://user-images.githubusercontent.com/48925593/167685752-ced6d2d3-c8ad-47c7-90e4-e51eb16163c9.png)


## **Step 5. Generate Discovery ISO**

Select ‘**Generate Discovery ISO**’; optionally change the selection for a Full image file, or a Minimal image file.

![image](https://user-images.githubusercontent.com/48925593/167685807-30250e5e-17db-40ce-9ce7-6cba8d38bef5.png)

 
## **Step 6.  Download Discovery ISO**

To download the new Discovery ISO file, select ‘Download Discovery ISO’.  
When complete, select ‘**Close**’.  

![image](https://user-images.githubusercontent.com/48925593/167685857-ff3596f7-0558-4203-a1c7-3ebeb73837df.png)


## **Step 7.  Boot Host to Discovery ISO & Install**

Boot new host server(s) from the new Discovery ISO, then continue with the process when they’ve been discovered by selecting ‘Install ready hosts’.  
Follow the installation progress, by optionally selecting ‘**View cluster events**’.

![image](https://user-images.githubusercontent.com/48925593/167685961-ff76a8a0-a817-4117-9bb1-c8458d1cdf66.png)


## **Step 8. Complete Installation**

When complete, the installer will show a status of ‘**installed**’.  
The Cluster Events will show a message: 
“Please check console for progress and to possibly approve pending CSRs)”


## **Step 9. Approve CSRs**

Login to the OpenShift console and navigate to Compute > Nodes and select the new host, and select ‘**Approve**’.
You can also use the oc command line utility to approve the pending CSR request.

![image](https://user-images.githubusercontent.com/48925593/167686103-7df56f8d-adcc-4ab6-8ab4-e534fcf9fd04.png)


## **Step 10. Approve any additional CSR’s**

![image](https://user-images.githubusercontent.com/48925593/167686169-9b0b9be8-e499-433e-bf76-72319491c19e.png)


## **Step 10. Complete. Node Ready**

When this process is complete, the new host should be in a ‘**Ready**’ state.  

![image](https://user-images.githubusercontent.com/48925593/167686230-30649909-2054-40fd-96a7-a3f4b85db55a.png)


