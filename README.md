# graphQL-learning

## API
Application Programming Interface

### Interface
상호작용 with whatever.
개발자, 제작자가 사용자에게 노출한 기능.

## REST / GraphQL

목적: communication.

차이점: 어떻게 노출되어 있는지.

### REST

서버와의 통신: "URL"로 이루어짐.

example )

api.notion.com/v1/pages/

api.notion.com/v1/databases/relationID/query/

-> **Organized, Comprehensible**

#### HTTP Method

**Communicate intention**

create, delete, update etc.

-> 같은 url을 보내더라도 백엔드 server가 그 의도를 파악해 행동을 함.

Get : receive what I want

POST : create what I want

PUT : update what I want

DELETE : (literally) delete what I want

PATCH : modify what I want

### GraphQL

**SPECIFICATION**

Reason of being | 존재의 이유

: REST의 문제점 해결

#### REST의 문제점

1. Over-fetching

필요하지 않은 너무 많은 data.

-> 해결: 필요한 것만을 요청. ``nothing more, nothing less.``

2. Underfetching

받은 data에 무언가에 대한 ID가 포함될 경우,

그 ID의 정보가 무엇인지 알기 위해 새로운 "request"가 필요함.

-> 해결: ``single request``로 원하는 정보를 모두 얻을 수 있어야 함.

