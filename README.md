def is_eligible_to_vote(age, is_citizen):
    if age >= 18 and is_citizen:
        return "Eligible to vote"
    else:
        return "Not eligible to vote"

# Example usage
age = int(input("Enter your age: "))
citizenship = input("Are you a citizen? (yes/no): ").strip().lower()

is_citizen = citizenship == "yes"
result = is_eligible_to_vote(age, is_citizen)
print(result)
