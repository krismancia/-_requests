# -_requests
 Write a second query to determine the percentage of requests that are Accepted.

select(( select count (action_taken) from friend_request where action_taken = ‘Accepted’)*100/ (select count (action_taken) from friend_request)) from friend_request where action_taken = ‘Accepted’;

