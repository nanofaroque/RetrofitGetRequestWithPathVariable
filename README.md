# RetrofitGetRequestWithPathVariable

This pattern below shows how to add path variable with your url string. Let say you need to hit this url: 
/sports/param1/year/param2/teams    

@GET("/sports/{league}/year/{year}/teams")
    public void getTeamsInLeagueInYear(@Path("league")String  league,@Path("year")String year,Callback<TeamResponse> callback);
    
    
Retrofit PUT request with path Variable and body(multi parameter): 


@PUT("/users/{userId}")
public void putUserZipCode(@Path("userId") String userId, @QueryMap Map<String, String> param,Callback<AddLocationResponse> callback);

userId--> this is the url path variable
in the body of the request i am passing two parameter with key value pair in the map called "param"
callback--> is the response back after the successful request

Retrofit POST request with parameter: 

@FormUrlEncoded                                                    
@POST("/users/login")
    public void login(@Field("email") String email, @Field("password") String passWord, Callback<LoginData> loginDataCallback);
