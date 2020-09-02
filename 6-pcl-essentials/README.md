# 6 - PCL ESSENTIALS 

__Essential PCL Libraries that are used for fullfilling the req__
 



__FIX PASSTHROUGH OUTPUT__ 

``c++ 
// Create the filtering object
  pcl::PassThrough<pcl::PointXYZ> pass;
  pass.setInputCloud (cloud);
  pass.setFilterFieldName ("z");
  pass.setFilterLimits (0.0, 1.0);
  //pass.setFilterLimitsNegative (true);
  pass.filter (*cloud_filtered);
``