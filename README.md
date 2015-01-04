
# Chart.js for Meteor 

*Tested against Meteor v1.0.2.1*
*Updated to use latest Chartjs 1.0.1-beta4 version*

- Package version: v0.0.6

The minified JS file has been modified from the official version to fix issues with Meteor and the latest 1.0.1-beta2 changes.

Fixes:
1. Added Chart=this.Chart; at the end of the minified file to fix variable scoping issue (Meteor 0.6+).
2. Included section of un-minified chartjs code to minified version to workaround issue 'Uncaught SyntaxError: Unexpected token =' when js is loaded in browser (tested in Chrome, Firefox, Safari). 
  - If you find a better solution, please raise a pull request! 

# Example code of using Chart.js with Meteor

On the branch 'test' there is an example of how to use ChartJs with Meteor.

## Requirements

* Meteor
* NPM
* Meteorite

## How do I install this?

1. Install Meteorite `npm install -g meteorite`
2. Create Your project `mrt create mynewapp`
3. Add chartjs `mrt add chartjs`

## References

[Meteor](http://docs.meteor.com/)

[Meteorite](http://oortcloud.github.com/meteorite/)

[Atmosphere (Smart Packages)](https://atmosphere.meteor.com/wtf/package)

[Chart.js Documentation](http://www.chartjs.org/)

[Chart.js Code](https://github.com/nnnick/Chart.js)
