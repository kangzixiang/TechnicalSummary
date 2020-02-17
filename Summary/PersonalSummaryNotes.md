# Note
## C++ Com编程还需要详细了解！
COM组件有三个最基本的接口类，分别是IUnknown、IClassFactory、IDispatch
interface IUnknown
{
public:
    virtual HRESULT STDMETHODCALLTYPE QueryInterface(REFIID riid, _COM_Outptr_  void **ppvObject) = 0;
    virtual ULONG STDMETHODCALLTYPE AddRef( void) = 0;
    virtual ULONG STDMETHODCALLTYPE Release( void) = 0;
};
