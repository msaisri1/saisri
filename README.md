2025-04-06 00:20:39 /usr/local/lib/python3.10/site-packages/pydantic/_internal/_config.py:373: UserWarning: Valid config keys have changed in V2:
2025-04-06 00:20:39 * 'orm_mode' has been renamed to 'from_attributes'
2025-04-06 00:20:39   warnings.warn(message, UserWarning)
2025-04-06 00:20:39 Traceback (most recent call last):
2025-04-06 00:20:39   File "/usr/local/bin/uvicorn", line 8, in <module>
2025-04-06 00:20:39     sys.exit(main())
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/click/core.py", line 1161, in __call__
2025-04-06 00:20:39     return self.main(*args, **kwargs)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/click/core.py", line 1082, in main
2025-04-06 00:20:39     rv = self.invoke(ctx)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/click/core.py", line 1443, in invoke
2025-04-06 00:20:39     return ctx.invoke(self.callback, **ctx.params)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/click/core.py", line 788, in invoke
2025-04-06 00:20:39     return __callback(*args, **kwargs)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/uvicorn/main.py", line 412, in main
2025-04-06 00:20:39     run(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/uvicorn/main.py", line 579, in run
2025-04-06 00:20:39     server.run()
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/uvicorn/server.py", line 66, in run
2025-04-06 00:20:39     return asyncio.run(self.serve(sockets=sockets))
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/asyncio/runners.py", line 44, in run
2025-04-06 00:20:39     return loop.run_until_complete(main)
2025-04-06 00:20:39   File "uvloop/loop.pyx", line 1518, in uvloop.loop.Loop.run_until_complete
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/uvicorn/server.py", line 70, in serve
2025-04-06 00:20:39     await self._serve(sockets)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/uvicorn/server.py", line 77, in _serve
2025-04-06 00:20:39     config.load()
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/uvicorn/config.py", line 435, in load
2025-04-06 00:20:39     self.loaded_app = import_from_string(self.app)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/uvicorn/importer.py", line 19, in import_from_string
2025-04-06 00:20:39     module = importlib.import_module(module_str)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/importlib/__init__.py", line 126, in import_module
2025-04-06 00:20:39     return _bootstrap._gcd_import(name[level:], package, level)
2025-04-06 00:20:39   File "<frozen importlib._bootstrap>", line 1050, in _gcd_import
2025-04-06 00:20:39   File "<frozen importlib._bootstrap>", line 1027, in _find_and_load
2025-04-06 00:20:39   File "<frozen importlib._bootstrap>", line 1006, in _find_and_load_unlocked
2025-04-06 00:20:39   File "<frozen importlib._bootstrap>", line 688, in _load_unlocked
2025-04-06 00:20:39   File "<frozen importlib._bootstrap_external>", line 883, in exec_module
2025-04-06 00:20:39   File "<frozen importlib._bootstrap>", line 241, in _call_with_frames_removed
2025-04-06 00:20:39   File "/app/app/main.py", line 3, in <module>
2025-04-06 00:20:39     from app.api.routes import auth, users
2025-04-06 00:20:39   File "/app/app/api/routes/auth.py", line 26, in <module>
2025-04-06 00:20:39     def get_profile(current_user=Depends(get_current_user)):
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/routing.py", line 994, in decorator
2025-04-06 00:20:39     self.add_api_route(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/routing.py", line 933, in add_api_route
2025-04-06 00:20:39     route = route_class(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/routing.py", line 554, in __init__
2025-04-06 00:20:39     self.dependant = get_dependant(path=self.path_format, call=self.endpoint)
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/dependencies/utils.py", line 292, in get_dependant
2025-04-06 00:20:39     sub_dependant = get_param_sub_dependant(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/dependencies/utils.py", line 126, in get_param_sub_dependant
2025-04-06 00:20:39     return get_sub_dependant(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/dependencies/utils.py", line 162, in get_sub_dependant
2025-04-06 00:20:39     sub_dependant = get_dependant(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/dependencies/utils.py", line 285, in get_dependant
2025-04-06 00:20:39     param_details = analyze_param(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/dependencies/utils.py", line 488, in analyze_param
2025-04-06 00:20:39     field = create_model_field(
2025-04-06 00:20:39   File "/usr/local/lib/python3.10/site-packages/fastapi/utils.py", line 98, in create_model_field
2025-04-06 00:20:39     raise fastapi.exceptions.FastAPIError(
2025-04-06 00:20:39 fastapi.exceptions.FastAPIError: Invalid args for response field! Hint: check that <class 'sqlalchemy.orm.session.Session'> is a valid Pydantic field type. If you are using a return type annotation that is not a valid Pydantic field (e.g. Union[Response, dict, None]) you can disable generating the response model from the type annotation with the path operation decorator parameter response_model=None. Read more: https://fastapi.tiangolo.com/tutorial/response-model/
