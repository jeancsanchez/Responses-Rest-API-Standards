# Common REST API Error Codes 
<div class="content">
<p class="lf-text-block lf-block" data-lf-anchor-id="8b890c4d5f9b2cbb2d05e85703116ad1:0">The error codes listed in the following table may be returned by an operation on any of the storage services.  <span class="lf-thread-btn"><a class="fycon-action-view" tabindex="0" aria-label="Write a Sidenote" data-lf-anchor-id="8b890c4d5f9b2cbb2d05e85703116ad1:0">+
</a>
</span></p>
<table>
<thead>
<tr>
<th>Error code</th>
<th>HTTP status code</th>
<th>User message</th>
</tr>
</thead>
<tbody>
<tr>
<td>ConditionNotMet</td>
<td>Not Modified (304)</td>
<td>The condition specified in the conditional header(s) was not met for a read operation.</td>
</tr>
<tr>
<td>MissingRequiredHeader</td>
<td>Bad Request (400)</td>
<td>A required HTTP header was not specified.</td>
</tr>
<tr>
<td>MissingRequiredXmlNode</td>
<td>Bad Request (400)</td>
<td>A required XML node was not specified in the request body.</td>
</tr>
<tr>
<td>UnsupportedHeader</td>
<td>Bad Request (400)</td>
<td>One of the HTTP headers specified in the request is not supported.</td>
</tr>
<tr>
<td>UnsupportedXmlNode</td>
<td>Bad Request (400)</td>
<td>One of the XML nodes specified in the request body is not supported.</td>
</tr>
<tr>
<td>InvalidHeaderValue</td>
<td>Bad Request (400)</td>
<td>The value provided for one of the HTTP headers was not in the correct format.</td>
</tr>
<tr>
<td>InvalidXmlNodeValue</td>
<td>Bad Request (400)</td>
<td>The value provided for one of the XML nodes in the request body was not in the correct format.</td>
</tr>
<tr>
<td>MissingRequiredQueryParameter</td>
<td>Bad Request (400)</td>
<td>A required query parameter was not specified for this request.</td>
</tr>
<tr>
<td>UnsupportedQueryParameter</td>
<td>Bad Request (400)</td>
<td>One of the query parameters specified in the request URI is not supported.</td>
</tr>
<tr>
<td>InvalidQueryParameterValue</td>
<td>Bad Request (400)</td>
<td>An invalid value was specified for one of the query parameters in the request URI.</td>
</tr>
<tr>
<td>OutOfRangeQueryParameterValue</td>
<td>Bad Request (400)</td>
<td>A query parameter specified in the request URI is outside the permissible range.</td>
</tr>
<tr>
<td>RequestUrlFailedToParse</td>
<td>Bad Request (400)</td>
<td>The url in the request could not be parsed.</td>
</tr>
<tr>
<td>InvalidUri</td>
<td>Bad Request (400)</td>
<td>The requested URI does not represent any resource on the server.</td>
</tr>
<tr>
<td>InvalidHttpVerb</td>
<td>Bad Request (400)</td>
<td>The HTTP verb specified was not recognized by the server.</td>
</tr>
<tr>
<td>EmptyMetadataKey</td>
<td>Bad Request (400)</td>
<td>The key for one of the metadata key-value pairs is empty.</td>
</tr>
<tr>
<td>InvalidXmlDocument</td>
<td>Bad Request (400)</td>
<td>The specified XML is not syntactically valid.</td>
</tr>
<tr>
<td>Md5Mismatch</td>
<td>Bad Request (400)</td>
<td>The MD5 value specified in the request did not match the MD5 value calculated by the server.</td>
</tr>
<tr>
<td>InvalidMd5</td>
<td>Bad Request (400)</td>
<td>The MD5 value specified in the request is invalid. The MD5 value must be 128 bits and Base64-encoded.</td>
</tr>
<tr>
<td>OutOfRangeInput</td>
<td>Bad Request (400)</td>
<td>One of the request inputs is out of range.</td>
</tr>
<tr>
<td>InvalidAuthenticationInfo</td>
<td>Bad Request (400)</td>
<td>The authentication information was not provided in the correct format. Verify the value of <code>Authorization</code> header.</td>
</tr>
<tr>
<td>InvalidInput</td>
<td>Bad Request (400)</td>
<td>One of the request inputs is not valid.</td>
</tr>
<tr>
<td>InvalidMetadata</td>
<td>Bad Request (400)</td>
<td>The specified metadata is invalid. It includes characters that are not permitted.</td>
</tr>
<tr>
<td>InvalidResourceName</td>
<td>Bad Request (400)</td>
<td>The specifed resource name contains invalid characters.</td>
</tr>
<tr>
<td>MetadataTooLarge</td>
<td>Bad Request (400)</td>
<td>The size of the specified metadata exceeds the maximum size permitted.</td>
</tr>
<tr>
<td>ConditionHeadersNotSupported</td>
<td>BadRequest (400)</td>
<td>Condition headers are not supported.</td>
</tr>
<tr>
<td>MultipleConditionHeadersNotSupported</td>
<td>Bad Request (400)</td>
<td>Multiple condition headers are not supported.</td>
</tr>
<tr>
<td>AuthenticationFailed</td>
<td>Forbidden (403)</td>
<td>Server failed to authenticate the request. Make sure the value of the <code>Authorization</code> header is formed correctly including the signature.</td>
</tr>
<tr>
<td>InsufficientAccountPermissions</td>
<td>Forbidden (403)</td>
<td>Read operations are currently disabled.</td>
</tr>
<tr>
<td>InsufficientAccountPermissions</td>
<td>Forbidden (403)</td>
<td>Write operations are not allowed.</td>
</tr>
<tr>
<td>ResourceNotFound</td>
<td>Not Found (404)</td>
<td>The specified resource does not exist.</td>
</tr>
<tr>
<td>AccountIsDisabled</td>
<td>Forbidden (403)</td>
<td>The specified account is disabled.</td>
</tr>
<tr>
<td>InsufficientAccountPermissions</td>
<td>Forbidden (403)</td>
<td>The account being accessed does not have sufficient permissions to execute this operation.</td>
</tr>
<tr>
<td>UnsupportedHttpVerb</td>
<td>Method Not Allowed (405)</td>
<td>The resource doesn't support the specified HTTP verb.</td>
</tr>
<tr>
<td>AccountAlreadyExists</td>
<td>Conflict (409)</td>
<td>The specified account already exists.</td>
</tr>
<tr>
<td>AccountBeingCreated</td>
<td>Conflict (409)</td>
<td>The specified account is in the process of being created.</td>
</tr>
<tr>
<td>ResourceAlreadyExists</td>
<td>Conflict (409)</td>
<td>The specified resource already exists.</td>
</tr>
<tr>
<td>ResourceTypeMismatch</td>
<td>Conflict (409)</td>
<td>The specified resource type does not match the type of the existing resource.</td>
</tr>
<tr>
<td>MissingContentLengthHeader</td>
<td>Length Required (411)</td>
<td>The <code>Content-Length</code> header was not specified.</td>
</tr>
<tr>
<td>ConditionNotMet</td>
<td>Precondition Failed (412)</td>
<td>The condition specified in the conditional header(s) was not met for a write operation.</td>
</tr>
<tr>
<td>RequestBodyTooLarge</td>
<td>Request Entity Too Large (413)</td>
<td>The size of the request body exceeds the maximum size permitted.</td>
</tr>
<tr>
<td>InvalidRange</td>
<td>Requested Range Not Satisfiable (416)</td>
<td>The range specified is invalid for the current size of the resource.</td>
</tr>
<tr>
<td>InternalError</td>
<td>Internal Server Error (500)</td>
<td>The server encountered an internal error. Please retry the request.</td>
</tr>
<tr>
<td>OperationTimedOut</td>
<td>Internal Server Error (500)</td>
<td>The operation could not be completed within the permitted time.</td>
</tr>
<tr>
<td>ServerBusy</td>
<td>Service Unavailable (503)</td>
<td>The server is currently unable to receive requests. Please retry your request.</td>
</tr>
</tbody>
</table>
</div>
