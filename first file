1.sol:)def count_developers(lst):
    # Your code here
    return sum(x["language"] == "JavaScript" and x["continent"] == "Europe" for x in lst)

2.sol)def greet_developers(lst): 
    for x in lst:
        x["greeting"] = f"Hi {x['firstName']}, what do you like the most about {x['language']}?"
    return lst

3.sol)def is_ruby_coming(lst): 
    return any(x["language"] == "Ruby" for x in lst)

4.sol)def get_first_python(users):
    for data in users:
        if data['language'] == 'Python':
            return f'{data["first_name"]}, {data["country"]}'
    
    return 'There will be no Python developers'

5.sol)from collections import Counter
def count_languages(lst): 
    return Counter([d['language'] for d in lst])

6.sol)def is_same_language(lst): 
    return len(set(i["language"] for i in lst)) == 1

7.sol)def find_senior(lst): 
    # your code here
    
    max_age = max(developer['age'] for developer in lst)
    oldest_developers_list = [developer for developer in lst if developer['age'] == max_age]
    return oldest_developers_list

# Example usage:
    list1 = [
    {'firstName': 'Gabriel', 'lastName': 'X.', 'country': 'Monaco', 'continent': 'Europe', 'age': 49, 'language': 'PHP'},
    {'firstName': 'Odval', 'lastName': 'F.', 'country': 'Mongolia', 'continent': 'Asia', 'age': 38, 'language': 'Python'},
    {'firstName': 'Emilija', 'lastName': 'S.', 'country': 'Lithuania', 'continent': 'Europe', 'age': 19, 'language': 'Python'},
    {'firstName': 'Sou', 'lastName': 'B.', 'country': 'Japan', 'continent': 'Asia', 'age': 49, 'language': 'PHP'},
   ]

    result = oldest_developers(list1)
    print(result)


8.sol)def all_continents(lst): 
    return len(set(x["continent"] for x in lst)) == 5

9.sol)def all_age_groups_signed_up(list):
    required_age_groups = {'teens', 'twenties', 'thirties', 'forties', 'fifties', 'sixties', 'seventies', 'eighties', 'nineties', 'centenarian'}
    signed_up_age_groups = {str(developer['age'] // 10 * 10) + 's' for developer in list}
    return required_age_groups.issubset(signed_up_age_groups)
    result = all_age_groups_signed_up(list1)
    print(result)


10.sol)function addUsername(list) {
  // thank you for checking out the Coding Meetup kata :)


    const currentYear = new Date().getFullYear();

    return list.map(developer => {
        const birthYear = currentYear - developer.age;
        const username = `${developer.firstName.toLowerCase()}${developer.lastName[0].toLowerCase()}${birthYear}`;
        
        return { ...developer, username };
    });
}


var list1 = [
    { firstName: 'Emily', lastName: 'N.', country: 'Ireland', continent: 'Europe', age: 30, language: 'Ruby' },
    { firstName: 'Nor', lastName: 'E.', country: 'Malaysia', continent: 'Asia', age: 20, language: 'Clojure' }
];

var updatedList = addUsername(list1);
console.log(updatedList);




11.sol)def get_average(lst): 
    return round(sum(x["age"] for x in lst) / len(lst))


12.sol)def find_admin(lst, lang): 
    return [i for i in lst if i['language']==lang and i['githubAdmin']=='yes']


13.sol)def is_language_diverse(lst): 
    # your code here
    language_counts = {'Python': 0, 'Ruby': 0, 'JavaScript': 0}

    for developer in lst:
        language_counts[developer['language']] += 1

    max_count = max(language_counts.values())
    total_remaining_count = sum(language_counts.values()) - max_count
    return max_count <= 2 * total_remaining_count
    result = is_language_diverse(list1)
    print(result)


14.sol)from collections import Counter
      def order_food(lst): 
    return Counter(dev['meal'] for dev in lst)


15.sol)def find_odd_names(lst): 
    # your code here
    odd_names = []
    for developer in lst:
        ascii_sum = sum(ord(char) for char in developer['firstName'])
        if ascii_sum % 2 != 0:
            odd_names.append(developer)

    return odd_names
    result = find_odd_names(list1)
    print(result)



16.sol)function askForMissingDetails(list) {
  // thank you for checking out the Coding Meetup kata :)
    const result = [];
    for (const developer of list) {
        const missingProperties = [];
        for (const property in developer) {
            if (developer[property] === null) {
                missingProperties.push(property);
            }
        }

        if (missingProperties.length > 0) {
            const question = `Hi, could you please provide your ${missingProperties.join(' and ')}.`;
            const developerWithQuestion = { ...developer, question };
            result.push(developerWithQuestion);
        }
    }
    return result;
}
var list1 = [
  { firstName: null, lastName: 'I.', country: 'Argentina', continent: 'Americas', age: 35, language: 'Java' },
  { firstName: 'Lukas', lastName: 'X.', country: 'Croatia', continent: 'Europe', age: 35, language: null },
  { firstName: 'Madison', lastName: 'U.', country: 'United States', continent: 'Americas', age: 32, language: 'Ruby' } 
];

var result = askForMissingDetails(list1);
console.log(result);



17.sol)def sort_by_language(arr):
	return sorted(arr, key=lambda x: (x["language"], x["first_name"]))
