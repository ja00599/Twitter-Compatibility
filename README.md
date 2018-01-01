# Twitter-Compatibility
Twitter compatibility checker
%Initialisation
clear,clc,close all
credentials=struct('ConsumerKey','Not defined','ConsumerSecret','Not defined','AcessToken','Not defined','AccessTokenSecret','Not defined');
 
%Taking input from user using their credentials
disp(Enter the following credentials :'); disp('');
credentials.ConsumerKey=input('Consumer Key :','s');
credentials.ConsumerSecret=input('Consumer Secret :','s');
credentials.AccessToken=input('Access Token :','s');
credentials.AccessTokenSecret=input('Access Token Secret :','s');
 
% creating twitty object
tw = twitty(credentials);
