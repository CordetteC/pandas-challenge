This homework was completed with the help of Xpert learning assistant for the lines of code below:
# Calculate the total budget. So for each unique school, add the budget to the cumulative disctrict budget.
unique_school_budget = school_data_combined[['school_name', 'budget']].drop_duplicates() #from Xpert Learning Assistant, creates df of only unique school/budget combos

# Formatting 
district_summary["Total Students"] = district_summary["Total Students"].map("{:,}".format)
district_summary["Total District Budget"] = district_summary["Total District Budget"].map("${:,.0f}".format)
district_summary["Average Math Score"] = district_summary["Average Math Score"].map("{:,.2f}".format)
district_summary["Average Reading Score"] = district_summary["Average Reading Score"].map("{:,.2f}".format)
district_summary["% Passing Math"] = district_summary["% Passing Math"].map("{:,.2f}%".format)
district_summary["% Passing Reading"] = district_summary["% Passing Reading"].map("{:,.2f}%".format)
district_summary["% Overall Passing"] = district_summary["% Overall Passing"].map("{:,.2f}%".format)
