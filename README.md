# Az_storage_cost_optimize_perf
Optimize performance and cost of Azure Disk Storage 

What is VM I/O capping: 

Let’s say, our app is requesting a certain amount of throughput and IOPS that the disk can manage, but the VM can't accommodate these requirements (a sort of compatibility between the VM and the underlying disk). 

(a) If you don't size the VM correctly for the storage performance an application requires, the VM itself becomes a bottleneck. In the below case, you can see our Disk is capable of delivering up to 900 MB/s but the OS has a hard limit of 1152 MB/s.  

 ![image](https://github.com/Maheshk-MSFT/Az_storage_cost_optimize_perf/assets/61469290/1d9206d2-2eee-481e-a979-1892f2194e2e)


(b) If you don't size the VM correctly for the storage performance an application requires, the Disks can also become a bottleneck. In this case, you can see our VM is capable of delivering up to 1152 MB/s but the underlying disk P30 can support only 200 MB/s.  

 
![image](https://github.com/Maheshk-MSFT/Az_storage_cost_optimize_perf/assets/61469290/004096f6-193e-4c5d-8350-4b1ef9d9b0a6)
