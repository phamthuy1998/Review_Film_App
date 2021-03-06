##
# Week 1 Project: Flicks
http://learning.coderschool.vn/course_images/_intro_to_android/movie_db1.gif
![image](https://user-images.githubusercontent.com/32641436/77922238-01106280-72cb-11ea-95a5-ce29d52b5f49.png)
![image](https://user-images.githubusercontent.com/32641436/77922759-aaefef00-72cb-11ea-8497-ac7096b40024.png)

**Overview** : Build a read-only movie listing app using the Movie Database API.

- The Movie Database [API documentation](https://developers.themoviedb.org/3/getting-started/introduction)
- Download the [JSONView extension](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc?hl=en) to view JSON better in your browser.
- Sample API Request: [https://api.themoviedb.org/3/movie/now\_playing?api\_key=a07e22bc18f5cb106bfe4cc1f83ad8ed](https://api.themoviedb.org/3/movie/now_playing?api_key=a07e22bc18f5cb106bfe4cc1f83ad8ed)
- Trailers API response: [https://api.themoviedb.org/3/movie/209112/trailers?api\_key=a07e22bc18f5cb106bfe4cc1f83ad8ed](https://api.themoviedb.org/3/movie/209112/trailers?api_key=a07e22bc18f5cb106bfe4cc1f83ad8ed)

**Libraries:**  Completing this project, requires the use of the [retrofit](https://guides.codepath.com/android/Consuming-APIs-with-Retrofit) and the [Glide](https://github.com/bumptech/glide) libraries. Add dependencies for these libraries to the [app/build.gradle](https://github.com/codepath/android-rest-client-template/blob/master/app/build.gradle#L30-L32) file.

- Be sure to  **include a README**  containing a GIF walkthrough of your app.
- Use [this README template](https://drive.google.com/open?id=1KShhsBlNorK4xzNLk-sMxNPGln2Ziin0) in order to have a complete README.

**User Stories** :

The following user stories  **must**  be completed:

- User can view a list of movies (title, poster image, and overview) currently playing in theaters from the Movie Database API.
- Lists should be fully optimized for performance with [Recyclerview](https://guides.codepath.com/android/Using-the-RecyclerView).
- Views should be responsive for both [landscape/portrait mode](http://guides.codepath.com/android/Understanding-App-Resources#creating-alternate-resources).
  - In portrait mode, the poster image, title, and movie overview is shown.

-
![image](https://user-images.githubusercontent.com/32641436/77922796-b7744780-72cb-11ea-922c-af4ad38f9bed.png)

  - In landscape mode, the rotated layout should use the backdrop image instead and show the title and movie overview to the right of it.
- ![image](https://user-images.githubusercontent.com/32641436/77922902-dffc4180-72cb-11ea-9c62-0bb6e17687f9.png)

The following advanced user stories are  **optional**  but recommended:

- Add pull-to-refresh for popular stream with [SwipeRefreshLayout](http://guides.codepath.com/android/Implementing-Pull-to-Refresh-Guide) ( **1 point** )
- Display a nice default placeholder graphic for each image during loading (read more about [Glide](https://github.com/bumptech/glide)) ( **1 point** )
- Improve the [user interface](http://guides.codepath.com/android/Styling-UI-Screens-FAQ#actionbar) through styling and coloring ( **1 to 5 points** _ depending on the difficulty of UI improvements_)
- For popular movies (i.e. a movie voted for more than 5 stars), the full backdrop image is displayed. Otherwise, a poster image, the movie title, and overview is listed. Use [Heterogenous RecyclerViews](https://guides.codepath.com/android/Heterogenous-Layouts-inside-RecyclerView) and use different ViewHolder layout files for popular movies and less popular ones. ( **2 points** )
- **Stretch:**  Expose details of movie (ratings using RatingBar, popularity, and synopsis) in a [separate activity.](http://guides.codepath.com/android/Using-Intents-to-Create-Flows#passing-data-to-launched-activities) ( **3 points** )
- **Stretch:**  Allow video posts to be played in full-screen using the [YouTubePlayerView](http://guides.codepath.com/android/Streaming-Youtube-Videos-with-YouTubePlayerView) ( **2 points** )
  - When clicking on a popular movie (i.e. a movie voted for more than 5 stars) the video should be played immediately.
  - Less popular videos rely on the detailed page should show an image preview that can initiate playing a YouTube video.
  - See the [trailers API](http://docs.themoviedb.apiary.io/#reference/movies/movieidvideos/get) for video information. Here&#39;s a [sample request](https://api.themoviedb.org/3/movie/209112/trailers?api_key=a07e22bc18f5cb106bfe4cc1f83ad8ed).
- **Stretch:**  Add a play icon overlay to popular movies to indicate that the movie can be played ( **1 point** ).
- **Stretch:**  Leverage the [data binding support module](http://guides.codepath.com/android/Applying-Data-Binding-for-Views) to bind data into one or more activity layout templates. ( **1 point** )
- **Stretch:**  Apply the popular [ButterKnife annotation library](http://guides.codepath.com/android/Reducing-View-Boilerplate-with-Butterknife) to reduce view boilerplate. ( **2****  point**)
- **Stretch:**  Add a rounded corners for the images using the [Picasso transformations](https://guides.codepath.com/android/Displaying-Images-with-the-Picasso-Library#other-transformations) or [Glide transformations](https://github.com/wasabeef/glide-transformations). ( **1 point** )
