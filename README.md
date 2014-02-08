There are 6 different attributes per question in the json file:
	"title": Is what will be displayed as H3 above the question.
	"type": Indicates one of three different types of questions.
		"pickOne" provides two or more questions and the user must pick one.
		"rearrangeList" provides a list of statements which must be placed in the correct order.
		"rearrangeBlock" is similar to lists but with potential for column sets. Items 
	"situation": An optional category which provides non-header pre-question text.
	"key": A string of numbers which will be used to evaluate answers. Starts at 1 (11 for columns).
		For "pickOne" the key will be the number of the correct data value.
		For "rearrangeList" the key will be a string which readjusted list items should form.
		For "rearrangeBlock" the key works similarly to 'rearrangeList'.
	"aceit": Provides the option for content within a text file to be displayed with Ace Editor, the default dimensions are 100% width and 350px height. Also default is text-editing disabled. This is currently configured to only access local files using AJAX.
	"data": Either an array (as in the case of 'pickOne' and 'rearrangeList') or a set object pairs (as in 'rearrangeBlock'). This where the questions/statments are written out.

To be developed:
	Relatively easily:
		"pickSome": A multiple choice set.
		"sortbyCategory": Changing rearrangeBlock to a sort-by-category type question. Currently can be sorted but not verified.
		Make columns in rearrangeBlock to be customizable.
	Somewhat challenging:
		"showAnswer": A section which contains answer information after the questions.
	Difficult but worthwhile:
		Text input questions which can be checked. Possibly using Ace Editor.
		GUI for easily making new JSON file quizlets.
