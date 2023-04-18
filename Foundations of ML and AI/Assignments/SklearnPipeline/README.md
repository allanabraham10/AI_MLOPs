## Learning Objectives

At the end of the experiment, we will be able to:
- appreciate the significance of a pipeline and its optimization
- setup a machine learning pipeline
- optimize the pipeline
- know techniques to analyze the results of optimization

## Information

A machine learning pipeline can be created by putting together a sequence of steps involved in training a machine learning model. It can be used to automate a machine learning workflow. The pipeline can involve pre-processing, feature selection, classification/regression, and post-processing steps. More complex applications may need to fit in other necessary steps within this pipeline.
Substances in traditional fire-extinguishing techniques may leave chemical waste, harm human health and cause social and economic damages. Therefore research on fire-extinguishing using renewable energy sources is important. The impact of sound waves on flame and combustion behavior of fuel is a common. Fire is a chemical reaction that breaks out with the combination of heat, fuel, and oxygen components. The heat, gas, and smoke resulting from this oxidation reaction may significantly harm to human and the environment. Early intervention to the fire facilitates to extinguish. However, depending on the scale of the fire and the fuel type, fire-extinguishing agents may vary. These substances in traditional fire-extinguishing techniques may leave chemical waste and harm human health. Additionally, it can also cause social and economic damages. In order to eliminate these impacts, researches on fire-extinguishing with renewable energy sources have been carried out. Currently, the impact of sound waves on flame and combustion behavior of fuel is a common research topic. The pressure changes in the air as a result of the sound waves lead to the occurrence of airflow. This airflow changes the behavior of the flame, fuel, and oxygen in the environment. The airflow created by the sound waves enables the fuel to spread over a wider surface. At this phase, the flame shows the tendency of spreading over a wide area together with the fuel. Fuel consumption also increases by the fuel particle oscillation due to the spread of flame and sound waves. While these stages are taking place, the air in the fire environment mixes and the amount of oxygen decreases as a result of the compression and expansion movements in the air. Through the combination of these three events, the flame can be extinguished. Necessary frequency ranges are available for the flame to be extinguished with the sound waves. Besides the frequency characteristic of sound waves, sound intensity level and the distance are also the factors having an impact on the ability to extinguish the flame.
Utilizing the fire characteristics, studies have been carried out to estimate the parameters necessary for the detection and extinguishing of the fire. The data have been obtained by examining the characteristics of the flames extinguished using sound waves. Statistical analysis and classification algorithms using these data provide information on the behaviour of the flame.


## Dataset

The dataset was obtained as a result of the extinguishing tests of four different fuel flames with a sound wave extinguishing system. The sound wave fire-extinguishing system consists of 4 subwoofers with a total power of 4,000 Watt placed in the collimator cabinet. There are two amplifiers that enable the sound come to these subwoofers as boosted. Power supply that powers the system and filter circuit ensuring that the sound frequencies are properly transmitted to the system is located within the control unit. While computer is used as frequency source, anemometer was used to measure the airflow resulted from sound waves during the extinguishing phase of the flame, and a decibel meter to measure the sound intensity. An infrared thermometer was used to measure the temperature of the flame and the fuel can, and a camera is installed to detect the extinction time of the flame. A total of 17,442 tests were conducted with this experimental setup.

The experiments are planned as follows:
- Three different liquid fuels and LPG fuel were used to create the flame.
- 5 different sizes of liquid fuel cans are used to achieve different size of flames.
- Half and full gas adjustment is used for LPG fuel.
- While carrying out each experiment, the fuel container, at 10 cm distance, was moved forward up to 190 cm by increasing the distance by 10 cm each time.
- Along with the fuel container, anemometer and decibel meter were moved forward in the same dimensions.
- Fire extinguishing experiments was conducted with 54 different frequency sound waves at each distance and flame size. Throughout the flame extinguishing experiments, the data obtained from each measurement device was recorded and a dataset was created.

The dataset includes following features:
SIZE: fuel container size representing the flame size
FUEL: fuel type
FREQUENCY
DECIBEL
DISTANCE
AIRFLOW
STATUS: flame extinction (dependent/target variable)

Accordingly, 6 input features and 1 output feature will be used in models. The explanation of a total of seven features for liquid fuels in the dataset is given in Table 1, and the explanation of 7 features for LPG fuel is given in Table 2. The status property (flame extinction or non-extinction states) can be predicted by using six features in the dataset. Status and fuel features are categorical, while other features are numerical. 8,759 of the 17,442 test results are the non-extinguishing state of the flame. 8,683 of them are the extinction state of the flame. According to these numbers, it can be said that the class distribution of the dataset is almost equal."
