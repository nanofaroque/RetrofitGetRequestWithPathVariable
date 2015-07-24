# RetrofitGetRequestWithPathVariable

@GET("/sports/{league}/year/{year}/teams")
    public void getTeamsInLeagueInYear(@Path("league")String  league,@Path("year")String year,Callback<TeamResponse> callback);
