# Coach
A tool for the detection of MVC based patterns in Android apps using classification

Data description:
We provide a dataset of 69 open-source Android apps collected from F-droid and manually annotated by two experts. The dataset was used in the paper “Classification based Architectural Patterns Detection in Android apps”. 
The dataset contains respectively 26, 11, 9 and 22 apps with MVC, MVP, MVVM and with no pattern.  We used an extended version of Paprika1 to compute code metrics. Please refer to the paper for the definition of code metrics.

Data format: 

Six sheets are in the CAPD dataset file:
- “apps” contains the names of the apps with the applied patterns in the form of “app_name |pattern” 
- “Model” contains the names of the apps followed by their model classes in the form of “app_name|model_class_1|model_class_2| … |”
- “Controller” contains code metrics of all the classes with Controller role in the dataset in the form of  “app_name | class_name  | NLIE | NLCEH | NNLCEH|NDMM        | NIMMM | npath_complexity |lack_of_cohesion_in_methods| number_of_methods| depth_of_inheritance |coupling_between_object_classes| class_complexity|                number_of_attributes| number_of_implemented_interfaces” 
- “Presenter” contains code metrics of all the classes with Presenter role in the dataset in the form of  “app_name | class_name  | NLIE | NLCEH | NNLCEH | NDMM      | NIMMM | npath_complexity |lack_of_cohesion_in_methods| number_of_methods| depth_of_inheritance |coupling_between_object_classes| class_complexity|number_of_attributes |number_of_implemented_interfaces”
- “ViewModel” contains code metrics of all the classes with ViewModel role in the dataset in the form of  “app_name | class_name  | NLIE | NLCEH | NNLCEH | NDMM | NIMMM | npath_complexity |lack_of_cohesion_in_methods| number_of_methods| depth_of_inheritance |coupling_between_object_classes| class_complexity|number_of_attributes |number_of_implemented_interfaces”
- “View” contains code metrics of all the classes with View role in the dataset in the form of “app_name | class_name  | NLIE | NLCEH | NNLCEH | NDMM | NIMMM | npath_complexity |lack_of_cohesion_in_methods| number_of_methods| depth_of_inheritance |coupling_between_object_classes| class_complexity|number_of_attributes |number_of_implemented_interfaces”
