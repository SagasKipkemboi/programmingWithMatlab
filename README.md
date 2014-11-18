programmingWithMatlab
=====================
clear all
clc
Amount=input('Give the amounts:') %Prompts the user to input the amount 
Currency=input('Give the currency in(USD, GBP, JPY):', 's');%promps the user to choose the currency

%These are the exchange rates 
rate_dollars=1.2112;
rate_pounds=0.68545; 
rate_yens=139.23;



if strcmp(Currency, 'USD')
       [dollars, average_d] = Exe2_Task_6(Amount, rate_dollars);
        disp('Initial Amount:')
        disp(Amount)
        disp('Currency choosen')
        disp(Currency)
        disp('Converted Amounts:')
        disp(dollars)
        disp(['Mean of the Converted Amount:' num2str(average_d)]);

elseif strcmp(Currency,'GBP')
        [pounds, average_p] = Exe2_Task_6(Amount, rate_pounds);
        disp('Initial Amount:')
        disp(Amount)
        disp('Currency choosen')
        disp(Currency)
        disp('Converted Amounts:')
        disp(pounds)
        disp(['Mean of the Converted Amount:' num2str(average_p)]);

elseif strcmp (Currency, 'JPY')
        [yens, average_y] = Exe2_Task_6(Amount, rate_yens);
        disp('Initial Amount:')
        disp(Amount)
        disp('Currency choosen')
        disp(Currency)
        disp('Converted Amounts:')
        disp(yens)
        disp(['Mean of the Converted Amount:' num2str(average_y)]);

else
    disp('Wrong Currency');
end
    
