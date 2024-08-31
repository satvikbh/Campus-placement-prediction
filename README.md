Student Placement Prediction
This project predicts whether a student will be recruited during campus placements based on various factors such as academic performance, work experience, and more. The project uses machine learning models to train on a dataset of student records and then evaluate and predict the placement outcomes.

Project Structure
train.csv: Contains the training dataset with the following columns:

sl_no: Serial number (not used in training)
gender: Gender of the student
ssc_p: Secondary Education percentage (10th Grade)
ssc_b: Board of Education for SSC (10th Grade)
hsc_p: Higher Secondary Education percentage (12th Grade)
hsc_b: Board of Education for HSC (12th Grade)
hsc_s: Specialization in HSC
degree_p: Degree percentage
degree_t: Undergraduate degree type
workex: Work experience
etest_p: Employability test percentage
specialisation: MBA specialization
mba_p: MBA percentage
status: Placement status (Placed or Not Placed)
salary: Salary offered (if placed)
test.csv: Contains the test dataset with the following columns:

sl_no: Serial number (not used in testing)
gender: Gender of the student
salary: Salary offered (if placed)
student_placement_predictions.csv: The output file that contains the predictions for the test set along with the actual status and predictions from different models.

Installation
To set up the environment for this project:

Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/student-placement-prediction.git
Navigate to the project directory:
bash
Copy code
cd student-placement-prediction
Install the required Python packages:
bash
Copy code
pip install -r requirements.txt
Usage
Training and Evaluation: The script trains multiple machine learning models on the train.csv dataset, evaluates them, and prints their performance metrics (Accuracy, Precision, Recall, F1 Score).

Prediction: After training, the script predicts whether students in the test.csv dataset will be placed and saves these predictions in student_placement_predictions.csv.
