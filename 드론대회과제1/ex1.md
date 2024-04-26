hour = hour + time;
while hour >= 24
    day = day + 1;
    hour = hour - 24;
end

if(month == 4 || month == 6 || month == 9 || month == 11)
    if(day > 30)
        month = month + 1;
        day = day - 30; 
    end
elseif(month == 2)
    if(day > 28) 
        month = month + 1;
        day = day - 28;
    end
else
    if(day > 31)
        month = month + 1;
        day = day - 31;
    end
end
