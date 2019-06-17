
close all
clear all
clc

load('church.mat');
label=CorrectIndex;
delta =0.5;
[index] = GFC_match(X,Y,delta);
[TP,FP,TN,FN, precision, recall, accuracy, corrRate]  = evaluatePR(label, index, size(X,1))

% Read images
ImgName1 = 'church1.jpg' ;
ImgName2 = 'church2.jpg' ;
I1 = imread(ImgName1) ;
I2 = imread(ImgName2) ;

% Plot results
plot_matches(I1, I2, X, Y, index, label);
