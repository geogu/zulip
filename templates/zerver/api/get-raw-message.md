# Get a raw message

{generate_api_description(/messages/{message_id}:get)}

## Usage examples

{start_tabs}
{tab|python}

{generate_code_example(python)|/messages/{message_id}:get|example}

{tab|curl}

{generate_code_example(curl)|/messages/{message_id}:get|example}

{end_tabs}

## Arguments

{generate_api_arguments_table|zulip.yaml|/messages/{message_id}:get}

## Response

#### Return values

* `raw_content`: The raw content of the message.

#### Example response

A typical successful JSON response may look like:

{generate_code_example|/messages/{message_id}:get|fixture(200)}

An example JSON response for when the specified message does not exist or it
is not visible to the user making the query (e.g. it was a PM between other
two users):

{generate_code_example|/messages/{message_id}:get|fixture(400)}
