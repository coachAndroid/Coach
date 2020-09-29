# Coach
A tool for the detection of MVC, MVP and MVVM patterns in Android apps using machine learning.

#Data description :

- “Dataset.xlsx” file provide a dataset of 69 open-source Android apps collected from F-droid and manually annotated by two experts. The dataset contains respectively 26, 11, 9 and 22 apps with MVC, MVP, MVVM and with no pattern. We used an extended version of Paprika to compute code metrics. 
- “Validation.xlsx” file provide the list of apps used for the validation of COACH. 

Please refer to the paper “Classification based Architectural Patterns Detection in Android apps” for more details.

#Data format:

Six sheets in “Dataset.xlsx” file: 
- “apps” contains the names of the apps with the applied patterns in the form of “app_name |pattern”
- “Model” contains the names of the apps followed by their model classes in the form of “app_name|model_class_1|model_class_2| … |”
- “Controller”  contains code metrics of all the classes with Controller role in the dataset in the form of “app_name|class_name|NLIE|NLCEH|NNLCEH|NDCM|NICM| npath_complexity|lack_of_cohesion_in_methods|number_of_methods|depth_of_inheritance|coupling_between_object_classes|class_complexity|number_of_attributes|number_of_implemented_interfaces”
- “Presenter” contains code metrics of all the classes with Presenter role in the dataset in the form of “app_name|class_name|NLIE|NLCEH|NNLCEH|NDCM|NICM| npath_complexity|lack_of_cohesion_in_methods|number_of_methods|depth_of_inheritance|coupling_between_object_classes|class_complexity|number_of_attributes|number_of_implemented_interfaces”
- “ViewModel” contains code metrics of all the classes with ViewModel role in the dataset in the form of “app_name|class_name|NLIE|NLCEH|NNLCEH|NDCM|NICM| npath_complexity|lack_of_cohesion_in_methods|number_of_methods|depth_of_inheritance|coupling_between_object_classes|class_complexity|number_of_attributes|number_of_implemented_interfaces”
- “View” contains code metrics of all the classes with View role in the dataset in the form of “app_name|class_name|NLIE|NLCEH|NNLCEH|NDCM|NICM| npath_complexity|lack_of_cohesion_in_methods|number_of_methods|depth_of_inheritance|coupling_between_object_classes|class_complexity|number_of_attributes|number_of_implemented_interfaces”


“Validation.xlsx” file contains the names of the apps with applied patterns in the form of “app_name |pattern”.
