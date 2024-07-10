# Music Company Sales Database Project

This project involves analyzing sales data from a music company. The data is organized into 11 tables, and various SQL queries were used to extract meaningful insights. The queries were written using PostgreSQL. Below is an overview of the database schema, followed by the specific questions addressed in the project.

## Database Schema

The database schema consists of the following tables:

**1. Artist:** ArtistId, Name

**2. Album:** AlbumId, Title, ArtistId

**3. Track:** TrackId, Name, AlbumId, MediaTypeId, GenreId, Composer, Milliseconds, Bytes, UnitPrice

**4. MediaType:** MediaTypeId, Name

**5. Genre:** GenreId, Name

**6. Playlist:** PlaylistId, Name

**7. PlaylistTrack:** PlaylistId, TrackId

**8. Employee:** EmployeeId, LastName, FirstName, Title, ReportsTo, BirthDate, HireDate, Address, City, State, Country, PostalCode, Phone, Fax, Email

**9. Customer:** CustomerId, FirstName, LastName, Company, Address, City, State, Country, PostalCode, Phone, Fax, Email, SupportRepId

**10. Invoice:** InvoiceId, CustomerId, InvoiceDate, BillingAddress, BillingCity, BillingState, BillingCountry, BillingPostalCode, Total

**11. InvoiceLine:** InvoiceLineId, InvoiceId, TrackId, UnitPrice, Quantity


![Schema](https://github.com/gagansaleria/SQL_Music_Database/assets/150334606/6090f110-620e-45c5-bc7b-90c60dd58c27)


## Questions

### Question Set 1

**Q1-** Who is the senior most employee based on job title?

**Q2-** Which countries have the most values?

**Q3-** What are the top 3 values of total invoices?

**Q4-** Which city has the best customers? We would like to throw a promotional Music Festival in the city we made the most money. Write a query that returns one city that has the highest sum of invoice totals. Return both the city name & sum of all invoice totals.

**Q5-** Who is the best customer? The customer who has spent the most money will be declared the best customer. Write a query that returns the person who has spent the most money.

### Question Set 2

**Q1-** Write query to return the email, first name, last name, & Genre of all Rock Music listeners. Return your list ordered alphabetically by email starting with A.

**Q2-** Let's invite the artists who have written the most rock music in our dataset. Write a query that returns the Artist name and total track count of the top 10 rock bands.

**Q3-** Return all the track names that have a song length longer than the average song length. Return the Name and Milliseconds for each track. Order by the song length with thelongest songs listed first.

### Question Set 3

**Q1-** Find how much amount spent by each customer on artists? Write a query to return customer name, artist name and total spent.

**Q2-** We want to find out the most popular music Genre for each country. We determine the most popular genre as the genre with the highest amount of purchases. Write a query that returns each country along with the top Genre. For countries where the maximum number of purchases is shared return all Genres.

**Q3-** Write a query that determines the customer that has spent the most on music for each country. Write a query that returns the country along with the top customer and how much they spent. For countries where the top amount spent is shared, provide all customers who spent this amount.
