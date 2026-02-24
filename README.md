
# J.Cole vs Kendrick Lamar, an analysis of who is the real "GOAT" of US Hip-Hop?

**Vedant Rajvanshi**

--------------------------

![J. Cole and Kendrick Lamar](https://wallpapers.com/images/hd/kendrick-lamar-and-j-cole-r81sbsqok781cpgx.jpg)


J. Cole and Kendrick Lamar are widely regarded as two of the most prominent contemporary US hip-hop artists. Both have released six studio albums over broadly similar time periods, consistently topping charts and accumulating multiple number-one singles. This project aims to assess which artist is more popular in Spotify terms, using Spotify API data to establish who really is the "GOAT" of US Hip-Hop.

We analyse two variables:

- **Spotify followers**: measured as each artist’s total number of Spotify followers.
- **Album popularity**: assessed by comparing the popularity scores of each artist’s six studio albums (i) album-by-album and (ii) via the average popularity score across all six albums.

Across three measures-(1) total followers, (2) individual album comparisons, and (3) average album popularity—the artist with the higher value on at least two out of three measures is identified as the overall winner.

### Conclusion

Overall, the Spotify data indicates that Kendrick Lamar is the more popular artist. Regarding **total followers** (Plot 1), the bar chart shows Kendrick has nearly 10 million more followers than J. Cole—a substantial difference. **Individual album comparisons** (Plot 2) are more favourable to J. Cole: the scatter plot indicates that three out of six of his albums score higher than Kendrick’s when comparing albums in release order. However, when considering **average album popularity** across all six studio albums (Plot 3), Kendrick’s discography performs slightly better, by roughly five percentage points on average.

With two of the three measures favouring Kendrick, **we conclude that Kendrick Lamar is more popular than J. Cole on Spotify**, and  ranks as the "GOAT" by the criteria used in this analysis.




### How to obtain Spotify API credentials

1. Go to the [Spotify API developer page](https://developer.spotify.com/) and either create an account or login to an existing Spotify account 
2. Go to the dashboard and from there create an app
    - Make sure to specify **Web API** as the API you are planning to use
3. Under 'Settings', you should now be able to see your Client ID and Client secret
4. In Nuvulus, ensure to create a .env file within your project directory to hide these credentials
    - Ensure to import the **python-dotenv** library
5. Finally, load the .env file and credentials to send a request to obtain your access token


### How to recreate the virtual Python Environment

To ensure you can run the code effectively and all relevant packages are installed use Python's built in venv module to recreate the virtual Python Environment



1. On the command line, change to your preferred working directory and use the following code to create a .venv virtual environment 

     ```
     python -m venv .venv
     ```


2. Next, activate the Virtual Environment

   On Windows run:

    ```
    .venv\Scripts\activate
    ```
       
   On MacOS or Linux run:
    ```
    source .venv/bin/activate
    ```



3. Finally install the required packages using the code:


    ```
    pip install -r requirements.txt
    ```

4. The following libraries should be installed:
- tqdm
- pandas
- lets-plot
- requests
- python-dotenv
- ipykernal
- sqlalchemy
