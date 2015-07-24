# RetrofitGetRequestWithPathVariable

This pattern below shows how to add path variable with your url string. Let say you need to hit this url: 
/sports/param1/year/param2/teams    

@GET("/sports/{league}/year/{year}/teams")
    public void getTeamsInLeagueInYear(@Path("league")String  league,@Path("year")String year,Callback<TeamResponse> callback);
