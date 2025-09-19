# comp163-personal-portfolio
# -------------------------
# Personal Information (strings)
# -------------------------
full_name = "Lauren Price"
student_email = "lcprice1@aggies.ncat.edu"
hometown = "Atlanta, GA"
graduation_semester = "Spring 2029"
major = "Computer Engineering "

# -------------------------
# Academic Data (lists)
# -------------------------
current_courses = ["COMP 163", "MATH 131", "GEEN 100", "CHEM 116", "DANC 200", "FRST101"]
completed_courses = ["Biology", "Psychology", "College Algebra", "Spanish III", "US History"]
credit_hours_list = [3, 4, 2, 1, 1, 1]  # corresponds to current_courses
gpa_history = [3.9, 3.9, 3.8, 3.9]  # semester GPAs as floats

# -------------------------
# Contact Information (tuples)
# Access tuple elements by index only as required
# -------------------------
emergency_contact = ("Mom", "Ywanda Price", "404-824-4762")
home_address = ("7227 Glen Cove Lane", "Stone Mountain, GA", "30087")
instagram_info = ("Instagram", "@laurennpricec", 1159)  # index 2 is follower count
twitter_info = ("Twitter", "@laurenpricec", 32)         # index 2 is follower count
birthday_info = ("Birthday", 1, 14, 2007)  # month, day, year in tuple indices 1..3

# -------------------------
# Interest Tracking (sets)
# -------------------------
current_skills_set = {"Python basics", "Cinematography", "Problem solving", "Time management", "Photography"}
skills_to_learn_set = {"JavaScript", "Data structures", "Git", "Web design", "Public speaking"}
career_interests_set = {"Software development", "Web development", "Data science", "Game development"}
hobbies_set = {"Dancing", "Photography", "Editing", "Sports", "Music"}
entertainment_backlog_set = {"Stranger Things", "Marvel", "The Vampire Diaries", "Moesha"}

# -------------------------
# Organizational Mapping (dictionaries)
# -------------------------
course_credits = {
    "COMP 163": 3,
    "MATH 313": 4,
    "GEEN 100": 2,
    "CHEM 116": 1,
    "DANC 200": 1,
    "FRST101": 1
}

course_professors = {
    "COMP 163": "Prof. Rhodes",
    "MATH 313": "Prof. Roop",
    "GEEN 100": "Prof. Alford",
    "CHEM 116": "Prof. Venkateswarlu",
    "DANC 200": "Prof. Stevens",
    "FRST101": "Prof. Painter"
}

course_rooms = {
    "COMP 163": "Gibbs 337",
    "MATH 313": "Marteena 216",
    "GEEN 100": "Grahm 210",
    "CHEM 116": "New Science Building 106",
    "DANC 200": "GCB 312",
    "FRST101": "Online"
}

monthly_budget = {
    "Food": 350,
    "Entertainment": 300,
    "Books": 125,
    "Transportation": 150
}

study_hours_per_subject = {
    "Programming": 10,
    "Calculus": 8,
    "Engineering": 8,
    "Chemistry": 6,
    "Dance": 3
    "College Success": 3
}

contact_directory = {
    "Mom": "404-824-4762",
    "Roommate": "336-555-7821",
    "Academic Advisor": "336-334-5000"
}

# -------------------------
# Required Calculations
# -------------------------
# a. Total current credits from credit_hours_list
total_current_credits = sum(credit_hours_list)

# b. Cumulative GPA from gpa_history list
# sum of semester GPAs divided by number of semesters (simple average)
cumulative_gpa = sum(gpa_history) / len(gpa_history)

# c. Count of completed courses
completed_courses_count = len(completed_courses)

# d. Total weekly study hours from study_hours_per_subject dictionary
total_weekly_study_hours = sum(study_hours_per_subject.values())

# e. Academic load (credits + study hours combined)
academic_load = total_current_credits + total_weekly_study_hours

# f. Monthly budget total from all categories
monthly_budget_total = sum(monthly_budget.values())

# g. Daily food budget (food amount ÷ 30, rounded to 2 decimals)
daily_food_budget = round(monthly_budget["Food"] / 30, 2)

# h. Annual budget projection (monthly total × 12)
annual_budget_projection = monthly_budget_total * 12

# i. Study cost per hour (books budget ÷ total study hours, rounded to 2 decimals)
# Note: if total_weekly_study_hours is 0 this would cause division by zero, but provided data is nonzero.
study_cost_per_hour = round(monthly_budget["Books"] / total_weekly_study_hours, 2)

# -------------------------
# Analytics Calculations
# -------------------------
# a. Total social media followers from platform tuples (index 2 in each tuple)
instagram_followers = instagram_info[2]
twitter_followers = twitter_info[2]
total_social_media_followers = instagram_followers + twitter_followers

# b. Skills count comparison (current vs. learning goals)
current_skills_count = len(current_skills_set)
skills_to_learn_count = len(skills_to_learn_set)

# c. Contact directory size analysis
contact_directory_size = len(contact_directory)

# d. Entertainment backlog management count
entertainment_backlog_count = len(entertainment_backlog_set)

# e. Academic workload assessment
# Provide numeric assessment: study hours per credit computed and rounded
study_hours_per_credit = round(total_weekly_study_hours / total_current_credits, 2)
