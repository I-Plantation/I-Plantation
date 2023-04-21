from flask import Flask, render_template, request

app = Flask(__name__)

# Define a function for shopping
@app.route('/shop', methods=['GET', 'POST'])
def shop():
    # Initialize a list of available products
    products = [("T-Shirt", 10), ("Jeans", 30), ("Jacket", 50)]
    
    # Initialize an empty shopping cart
    cart = []
    
    # Handle GET request
    if request.method == 'GET':
        # Render the shopping template with the available products
        return render_template('shopping.html', products=products)
    
    # Handle POST request
    elif request.method == 'POST':
        # Get the selected product from the form data
        product_id = int(request.form['product_id'])
        product = products[product_id - 1]
        
        # Add the selected product to the cart
        cart.append(product)
        
        # Display a message confirming that the product was added to the cart
        message = product[0] + " has been added to your cart."
        
        # Calculate the total cost of the items in the cart
        total = sum([item[1] for item in cart])
        
        # Render the shopping template with the updated cart and message
        return render_template('shopping.html', products=products, cart=cart, message=message, total=total)
    
    else:
        # Return an error message if the request method is not GET or POST
        return "Error: Invalid request method."

# Define a function for processing payment using Touch 'n Go
@app.route('/pay', methods=['POST'])
def pay():
    # Get the Touch 'n Go card number from the form data
    card_number = request.form['card_number']
    
    # Calculate the total cost of the items in the cart
    total = int(request.form['total'])
    
    # Process payment using Touch 'n Go
    if len(card_number) == 10 and card_number.isdigit():
        message = "Payment of RM" + str(total) + " has been successfully processed using Touch 'n Go card ending in " + card_number[-4:] + ". Thank you for shopping with us!"
    else:
        message = "Invalid card number."
    
    # Render the payment template with the payment status message
    return render_template('payment.html', message=message)

if __name__ == '__main__':
    app.run(debug=True)
