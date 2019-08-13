Following https://medium.com/@cplankey/use-lambda-layers-to-post-to-slack-513782db3d82

First cut is manual set-up as described in URL above.

Usage example:
const pts = require('posttoslack');
exports.handler = async(event, context) => {
    return pts.posttoslack("hooks.slack.com", "/services/T66G01W5R/BM6QPS9U6/NLiT5uYMrf3T320DTf5P3L5Z", "lambda says hello, @nickj");
};
