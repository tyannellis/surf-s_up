# surfs_up

## Purpose of Analysis 
The purpose of this analysis is to determine if the temperatures in July and December are good enough for a surf shop to be profitable. 

## Results 
- June has an average temperature of 74 degrees (+3 degrees more than December)
- June has a min temperature of 64 degrees (+8 degrees more than)
- The 25th percentile of the temperatures for June is 73 (+4 degrees mpre than December)

## Summary 
Overall the temperatures in June and December don't appear to be that different. Two more queries I would complete would be to see trends in raining for both months.   

results_june = session.query(Measurement.percipitation).\
 filter(extract('month',Measurement.date)==6).all()
 
 results_december = session.query(Measurement.percipitation).\
 filter(extract('month',Measurement.date)==12).all()
