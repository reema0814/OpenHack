# Challenge 2 - Use Machine Learning to Expose Data Issues

## Background story

Now that you have had a chance to explore the data now lets use Machine Learning to figure which portion of the data is creating the underlying issues. For this type of data issue we have chosen to use classification model. 

## Technical details

Create the following

- Create compute
- Create a dataset
- Create a pipeline in Designer and load data to canvas
- Add transformations
- Run the pipeline
- View the transformed data
- Add training modules
- Run the training pipeline
- Create an inference pipeline
- Deploy a service
- Test the service

## Success Criteria

Demonstrate to the coach that you are able to provide a sample json segment to show that it will properly predict either 0 or 1 based off the new service.

**Negative Return Prediction** 

```
{
	"Inputs": {
		"input1": [
			{
				"_KEY_OrderNo": 1028476,
				"_KEY_Supplier": 16,
				"ArticleNo": 502,
				"KEY_CustomerNo": 10752,
				"F_Discounts": 0,
				"F_VolumeDiscount": 0,
				"F_StudentDiscount": 0,
				"F_ListPrice": 33.99,
				"F_IsReturned": 0,
				"A_Category": "T-Shirt short",
				"S_Country": "USA",
				"C_MeansOfPayment": "direct debit",
				"C_Fit": "Regular",
				"F_IsDefect": 0,
				"C_City": "Berlin"
			}
		]
	},
	"GlobalParameters": {}
}
```

**Positive Return Prediction**
```
{
	"Inputs": {
		"input1": [
			{
				"_KEY_OrderNo": 477063,
				"_KEY_Supplier": 35,
				"ArticleNo": 568702,
				"KEY_CustomerNo": 805629,
				"F_Discounts": 1,
				"F_VolumeDiscount": 1,
				"F_StudentDiscount": 1,
				"F_ListPrice": 1886.79,
				"F_IsReturned": 0,
				"A_Category": "Accessoires",
				"S_Country": "France",
				"C_MeansOfPayment": "voucher",
				"C_Fit": "Fide",
				"F_IsDefect": 1,
				"C_City": "Regensburg"
			}
		]
	},
	"GlobalParameters": {}
}
```
## Resources

- https://microsoftlearning.github.io/AI-900-AIFundamentals/instructions/02b-create-classification-model.html
- https://learn.microsoft.com/en-us/azure/machine-learning/how-to-run-jupyter-notebooks?view=azureml-api-2
- [Explore classification with Azure Machine Learning Designer](https://microsoftlearning.github.io/AI-900-AIFundamentals/instructions/02b-create-classification-model.html)




