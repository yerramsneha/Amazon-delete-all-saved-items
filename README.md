# Amazon-delete-all-saved-items
Steps to delete all saved items in amazon
How to delete all the items from Amazon saved for later list
step-1:------------------Open the browser
step-2:---------------Navigate to Amazon.com
step-3:---------------Log in to your account
step-4:-----------Click the Amazon shopping basket in the top right corner
step-5:------------Scroll down to display the Saved for later items(only displayed items will delete)
step-6:------------Right Click any blank area of the webpage
step-7:------------click on console 
step-8:-----------------Copy the below code 
code: 
function deleteSavedItems() 
{
	var query = document.querySelectorAll("#sc-saved-cart input[value=Delete]")
	if (query.length) {
		query[0].click();
	}
	if (query.length > 1) 
  {
		setTimeout(deleteSavedItems,100);
	}
	else {
		console.log('Finished');
	}
}
deleteSavedItems();

step-9:--------------------Then paste the copied code above into the white text box on the developer console. To do this click the white text box and press Ctrl + V
Step-10:--------------------Press Enter to run the code and the items should start to disappear.
If this doesn’t work on the first try it is because copy and pasting the code renders quotes that are ASCII characters which are not correct. You’ll have to paste the code into the Console, then replace the quotes (4 of them) with quotes from your keyboard.
Use ‘ <– next to the Enter key.
