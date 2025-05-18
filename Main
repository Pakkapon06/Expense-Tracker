def add_expense(expense,amount, category):
    expense.append({'amount': amount, 'category': category})

def total_expense(expense):
    return sum(map( lambda expense:expense['amount'] , expense))

def filter_by_category(expense,category):
    return list(filter( lambda expense:expense['category'] == category , expense))

def main():
    expense = []
    while True:
        print(f'\nExpense Tracker\n1. Add Expense\n2. List All Expense\n3. Total Expense\n4. Filter expense by category\n5. Exiting the Program')
        choice = int(input('Enter you choice: '))

        if choice == 1:     
            amount = float(input('Enter Amount: '))
            category = input('Enter Category: ')
            add_expense(expense,amount,category)

        if choice == 2:
            print('\nAll Expense:')
            for i in expense:
                print(f'Amount: {i['amount']} , Category: {i['category']}')
            
        
        if choice == 3:
            print(f'\nTotal Expense: {total_expense(expense)}')
        
        if choice == 4:
            category = input('Enter category to filter: ')
            print(f'\nExpense for {category}')
            filtered = filter_by_category(expense,category)
            for i in filtered:
                print(f'Amount: {i['amount']} , Category: {i['category']}')
        
        if choice == 5:
            print('Exiting The Program')
            break

main()