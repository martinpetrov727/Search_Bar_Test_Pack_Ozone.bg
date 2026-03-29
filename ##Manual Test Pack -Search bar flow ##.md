## Manual Test Pack – Search Bar Flow  
App/Site: https://www.ozone.bg/  
Date: 11.03.2026  
Tester: Martin Petrov  

---

## Scope
Testing the search functionality and user experience for a guest user.

---

## Test Cases

### TC-001 - Search with valid keyword
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "iphone"
3. Click search

Expected Result:
- Relevant products related to "iPhone" are displayed


### TC-002 - Search with empty input
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Leave input empty
3. Click search

Expected Result:
- No search is performed OR page refreshes without results


### TC-003 - Search for unavailable product
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "PS3"
3. Click search

Expected Result:
- No unavailable products are displayed OR system shows no results message


### TC-004 - Search with special characters
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "@@@"
3. Click search

Expected Result:
- Error or "No results found" message is displayed
- Suggested products may appear


### TC-005 - Search with single character
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "A"
3. Click search

Expected Result:
- Products containing "A" are displayed


### TC-006 - Search with only space
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Press space
3. Click search

Expected Result:
- No results are shown OR validation message is displayed


### TC-007 - Search with numeric input
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "12345"
3. Click search

Expected Result:
- Products matching numeric input (e.g., IDs/barcodes) are displayed OR no results message


### TC-008 - Search with alphanumeric input
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "1abc"
3. Click search

Expected Result:
- Relevant results are displayed OR no results message appears


### TC-009 - Search with mixed invalid characters
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "@#1a"
3. Click search

Expected Result:
- No results found message is displayed


### TC-010 - Search with very long input
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Enter a string with 100+ characters
3. Click search

Expected Result:
- System handles input without crashing
- No results message or relevant results are displayed


### TC-011 - Search with leading space
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type " iphone"
3. Click search

Expected Result:
- Results for "iphone" are displayed (space is ignored)


### TC-012 - Search using Enter key
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "iphone"
3. Press Enter

Expected Result:
- Search results are displayed


### TC-013 - Search with partial keyword
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "iph"
3. Press Enter

Expected Result:
- Relevant products or suggestions are displayed


### TC-014 - Select from search suggestions
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar
2. Type "iph"
3. Click on a suggested item

Expected Result:
- User is redirected directly to the selected product page


### TC-015 - Search bar suggestion behavior
Preconditions:
- User is on the ozone.bg homepage

Steps:
1. Click on the search bar

Expected Result:
- Suggested products and categories are displayed