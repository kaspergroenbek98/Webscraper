# Webscraper for job application
A webscraper made for a job interview, where I have collected data from a book catalogue of a publisher from the firm i'm applying at.

The webscraber works by collecting the URL of the books from every page in the overall catalogue, then it accesses every individual page of the books and (by the use of regular expressiones, regex) finds the data I'm interested in.
The data that gets collected is:
- The title of the book
- Author(s)
- Release date
- Price
- Page count

Then it gets read into a dataframe, where the gender of the author is added by crosschecking lists (from excel files) of all man and female names in Denmark, if the name is bi-gender or has multiple authors of both genders, then it returns a Nonetype.
At the end it gets written into an excel file, where it can be used for visualisation in other software (Tableau in my case).
