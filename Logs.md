***
Ejemplo en Java
```
@ExceptionHandler(value = { Exception.class })
protected ResponseEntity<ApiError> handleUnknownException(Exception e) {
    LOGGER.error("Un log de error", e);
    LOGGER.info("Un log de info {save:$NUMBER_WAVES}");
    LOGGER.warn("Un log de warning");

    NewRelic.noticeError(e);

    ApiError apiError = new ApiError("internal_error", "Internal server error", HttpStatus.INTERNAL_SERVER_ERROR.value());
    return ResponseEntity.status(apiError.getStatus())
            .body(apiError);
}
```